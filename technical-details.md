# Technical Details

Hosting a MMM server is similar to hosting a static website, with the following differences:

1. The subdomain should be set to `mmm` (e.g. `mmm.example.com`).
2. All pages should end in with the `.md` extension, and should be served with the `text/markdown` MIME type.
3. The default page should be set to `index.md`.
4. These pages should, of course, use the [Markdown](markdown.md) format.

## Setup on AWS

You can host a static MMM server on AWS using S3 and CloudFront. Here are the steps:

1. **Create an S3 Bucket**: Create a new S3 bucket with the name `mmm.example.com` (replace with your domain).
2. **Upload Files**: Upload your Markdown files to the S3 bucket.
3. **Set Permissions**: Make the bucket public and set the appropriate permissions for the files.
4. **Create a CloudFront Distribution**: Create a CloudFront distribution with the S3 bucket as the origin.
5. **Set Default Root Object**: Set the default root object to `index.md`.
6. **Configure CNAME**: Add a CNAME record in your DNS settings to point `mmm.example.com` to the CloudFront distribution.
7. **Set MIME Type**: Ensure that the S3 bucket is configured to serve `.md` files with the `text/markdown` MIME type.
8. **Test**: Access your MMM server at `mmm.example.com` and verify that the Markdown files are rendered correctly.

Setting the default page to `index.md` for subdirectories requires you to add the following CloudFront function and associate it with your CloudFront distribution:

```javascript
async function handler(event) {
    var request = event.request;
    var uri = request.uri;
    
    // Check whether the URI is missing a file name.
    if (uri.endsWith('/')) {
        request.uri += 'index.md';
    } 
    // Check whether the URI is missing a file extension.
    else if (!uri.includes('.')) {
        request.uri += '/index.md';
    }

    return request;
}
```

[JLH](people.md)
