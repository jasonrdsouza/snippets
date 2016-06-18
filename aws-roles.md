# Using AWS Roles

Incantation to use boto with a specific profile from your `.aws/credentials` file:

```
import boto3

session = boto3.Session(profile_name='NAME_OF_PROFILE_IN_CREDENTIALS_FILE')
dynamoClient = session.client('dynamodb')
```

Using a profile in java:

````
import com.amazonaws.services.s3.AmazonS3Client
import com.amazonaws.auth.profile.ProfileCredentialsProvider

val s3Client = new AmazonS3Client(new ProfileCredentialsProvider("sandbox"))
```
