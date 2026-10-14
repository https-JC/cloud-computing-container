# Part 2: Short Answer
## Question 1 Explain why the uploader and viewer use separate IAM roles instead of one shared role with both permissions:  
Any system or application should utilize the principle of least privilege because the user only needs to view files it should only have read permissions. Likewise, a user that only needs to upload files should only have those permissions. Any instance where a user’s permissions are greater than what they need it increases the attack surface and can cause issues for security. 

## Question 2 Explain why embedding code directly into user-data means the instance never needs a Git or S3 credential just to fetch its own code:  
because the code is embedded into the instance when it boots it does not have to authenticate against external services like a private repository or a s3 bucket to download files It instead already has the files it needs.