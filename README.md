STATIC WEBSITE HOSTING
The primary objective of this project is to deploy a secure and scalable static web hosting solution on Amazon Simple Storage Service (S3) for an online book shopping web page. This deployment aims to showcase the simplicity and effectiveness of using AWS S3 to host static content, including HTML and CSS files, for an e-commerce application.

Key Steps To Be Followed:
	Create an S3 bucket to store and serve static files for your web page.
	Enable host a static website option 
	Configure access permissions for your S3 bucket, including a bucket policy that allows public read access to the necessary files.
	In AWS (Amazon Web Services), a policy is a set of permissions that define the actions allowed or denied on AWS resources.

  Policy:
{
    "Version": "2012-10-17",
    "Statement": [
    	{
        	"Sid": "PublicReadGetObject",
        	"Effect": "Allow",
        	"Principal": "*",
        	"Action": [
            	"s3:GetObject"
        	],
        	"Resource": [
                "arn:aws:s3:::mylostlibrary/*"
        	]
    	}
    ]
}

	Upload HTML, CSS and any other assets (images, etc.) that make up your static website.
	By accessing the URL you can demonstrate your static web site in the browser.
