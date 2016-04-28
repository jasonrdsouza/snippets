# Using Boto with AWS Roles

Incantation to use boto with a specific role in your `.aws/credentials` file.

```
import boto3

session = boto3.Session(profile_name='NAME_OF_PROFILE_IN_CREDENTIALS_FILE')
dynamoClient = session.client('dynamodb')

...
```

