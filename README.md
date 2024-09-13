{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "AllowPutBucketPolicy",
            "Effect": "Allow",
            "Principal": {
                "AWS": "arn:aws:iam::your-account-id:role/developers-pcluster-deploy-role"
            },
            "Action": "s3:PutBucketPolicy",
            "Resource": "arn:aws:s3:::your-bucket-name"
        }
    ]
}

{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "AllowPutBucketPolicy",
            "Effect": "Allow",
            "Action": "s3:PutBucketPolicy",
            "Resource": "arn:aws:s3:::your-bucket-name"
        }
    ]
}
