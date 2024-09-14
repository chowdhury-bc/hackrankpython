{
  "Version": "2012-10-17",
  "Id": "PolicyForDevelopersPClusterDeployRole",
  "Statement": [
    {
      "Sid": "AllowS3ActionsForSpecificRole",
      "Effect": "Allow",
      "Principal": {
        "AWS": "arn:aws:iam::123456789012:role/developers-pcluster-deploy-role"
      },
      "Action": [
        "s3:GetObject",
        "s3:PutObject",
        "s3:DeleteObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": [
        "arn:aws:s3:::my-pcluster-bucket",
        "arn:aws:s3:::my-pcluster-bucket/*"
      ]
    }
  ]
}

