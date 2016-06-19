# AWS CLI tricks

## Find and clean up incomplete multi-part uploads
```
# List incomplete uploads
aws --profile PROFILE_NAME s3api list-multipart-uploads --bucket BUCKET_NAME
# Abort incomplete uploads (and remove any temporary files)
aws --profile personal s3api abort-multipart-upload --bucket BUCKET_NAME --key KEY_NAME --upload-id UPLOAD_ID
```
