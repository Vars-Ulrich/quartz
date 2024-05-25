---
title: 
tags: 
icon: 
aliases: 
---
# [[API Gateway]]
##         lambda-code.py
```python
import json

def lambda_handler(event, context):
    body = "Hello from Lambda!"
    statusCode = 200
    return {
        "statusCode": statusCode,
        "body": json.dumps(body),
        "headers": {
            "Content-Type": "application/json"
        }
    }
```

# [[Command Line Interface]]
##         ec2-metadata.sh
```bash
#!/bin/bash
# example
curl http://169.254.169.254/latest/meta-data/instance-id
```

# [[CloudFormation]]
##         0-just-ec2.yaml
```yaml
---
Resources:
  MyInstance:
    Type: AWS::EC2::Instance
    Properties:
      AvailabilityZone: us-east-1a
      ImageId: ami-a4c7edb2
      InstanceType: t2.micro

```

##         1-ec2-with-sg-eip.yaml
```yaml
---
Parameters:
  SecurityGroupDescription:
    Description: Security Group Description
    Type: String

Resources:
  MyInstance:
    Type: AWS::EC2::Instance
    Properties:
      AvailabilityZone: us-east-1a
      ImageId: ami-a4c7edb2
      InstanceType: t2.micro
      SecurityGroups:
        - !Ref SSHSecurityGroup
        - !Ref ServerSecurityGroup

  # an elastic IP for our instance
  MyEIP:
    Type: AWS::EC2::EIP
    Properties:
      InstanceId: !Ref MyInstance

  # our EC2 security group
  SSHSecurityGroup:
    Type: AWS::EC2::SecurityGroup
    Properties:
      GroupDescription: Enable SSH access via port 22
      SecurityGroupIngress:
      - CidrIp: 0.0.0.0/0
        FromPort: 22
        IpProtocol: tcp
        ToPort: 22

  # our second EC2 security group
  ServerSecurityGroup:
    Type: AWS::EC2::SecurityGroup
    Properties:
      GroupDescription: !Ref SecurityGroupDescription
      SecurityGroupIngress:
      - IpProtocol: tcp
        FromPort: 80
        ToPort: 80
        CidrIp: 0.0.0.0/0
      - IpProtocol: tcp
        FromPort: 22
        ToPort: 22
        CidrIp: 192.168.1.1/32

Outputs:
  ElasticIP:
    Description: Elastic IP Value
    Value: !Ref MyEIP
```

# [[Elastic Block Store]]
##         commands.txt
```txt
See: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-using-volumes.html

See: https://www.unixmen.com/how-to-measure-disk-performance-with-fio-and-ioping/


```

# [[Elastic Cloud Compute|EC2]] Fundamentals
##         ec2-user-data.sh
```bash
#!/bin/bash
# Use this for your user data (script from top to bottom)
# install httpd (Linux 2 version)
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
echo "<h1>Hello World from $(hostname -f)</h1>" > /var/www/html/index.html
```

# [[Elastic File System]]
##         efs.sh
```bash
# on both instances:
sudo yum install -y amazon-efs-utils
sudo mkdir /efs
sudo mount -t efs fs-yourid:/ /efs

# you can now write files into /efs and they'll be available on both your ec2 instances!
```

# [[Kinesis]]
##         kinesis-data-streams.sh
```bash
#!/bin/bash

# get the AWS CLI version
aws --version

# PRODUCER

# CLI v2
aws kinesis put-record --stream-name test --partition-key user1 --data "user signup" --cli-binary-format raw-in-base64-out

# CLI v1
aws kinesis put-record --stream-name test --partition-key user1 --data "user signup"


# CONSUMER 

# describe the stream
aws kinesis describe-stream --stream-name test

# Consume some data
aws kinesis get-shard-iterator --stream-name test --shard-id shardId-000000000000 --shard-iterator-type TRIM_HORIZON

aws kinesis get-records --shard-iterator <>
```

# [[Key Management Service|KMS]]
##         ExampleSecretFile.sh
```txt
SuperSecretPassword
```

##         kms-demo-cli.sh
```bash
# 1) encryption
aws kms encrypt --key-id alias/tutorial --plaintext fileb://ExampleSecretFile.txt --output text --query CiphertextBlob  --region eu-west-2 > ExampleSecretFileEncrypted.base64

# base64 decode for Linux or Mac OS 
cat ExampleSecretFileEncrypted.base64 | base64 --decode > ExampleSecretFileEncrypted

# base64 decode for Windows
certutil -decode .\ExampleSecretFileEncrypted.base64 .\ExampleSecretFileEncrypted


# 2) decryption

aws kms decrypt --ciphertext-blob fileb://ExampleSecretFileEncrypted   --output text --query Plaintext > ExampleFileDecrypted.base64  --region eu-west-2

# base64 decode for Linux or Mac OS 
cat ExampleFileDecrypted.base64 | base64 --decode > ExampleFileDecrypted.txt


# base64 decode for Windows
certutil -decode .\ExampleFileDecrypted.base64 .\ExampleFileDecrypted.txt
```
# [[Route 53]]
##         user-data.sh
```bash
#!/bin/bash
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
EC2_AVAIL_ZONE=$(curl -s http://169.254.169.254/latest/meta-data/placement/availability-zone)
echo "<h1>Hello World from $(hostname -f) in AZ $EC2_AVAIL_ZONE </h1>" > /var/www/html/index.html
```

# [[Simple Storage Service|S3]]
##        CORS_CONFIG.json
```json
[
    {
        "AllowedHeaders": [
            "Authorization"
        ],
        "AllowedMethods": [
            "GET"
        ],
        "AllowedOrigins": [
            "<url of first bucket with http://...without slash at the end>"
        ],
        "ExposeHeaders": [],
        "MaxAgeSeconds": 3000
    }
]
```

beach.jpg
coffee.jpg
##         extra-page.html
```html
<p>This <strong>extra page</strong> has been successfully loaded!</p>
```

## index-with-fetch.html
```html
<html>
    <head>
        <title>My First Webpage</title>
    </head>
    <body>
        <h1>I love coffee</h1>
        <p>Hello world!</p>
    </body>

    <img src="coffee.jpg" width=500/>

    <!-- CORS demo -->
    <div id="tofetch"/>
    <script>
        var tofetch = document.getElementById("tofetch");

        fetch('http://<bucket URL>/extra-page.html')
        .then((response) => { 
            return response.text();
        })
        .then((html) => {
            tofetch.innerHTML = html     
        });
    </script>
</html>


```

## index.html
```html
<html>
    <head>
        <title>My First Webpage</title>
    </head>
    <body>
        <h1>I love coffee</h1>
        <p>Hello world!</p>
    </body>

    <img src="coffee.jpg" width=500/>

    <!-- CORS demo -->
    <div id="tofetch"/>
    <script>
        var tofetch = document.getElementById("tofetch");

        fetch('http://demo-other-origin-stephane.s3-website.ca-central-1.amazonaws.com/extra-page.html')
        .then((response) => { 
            return response.text();
        })
        .then((html) => {
            tofetch.innerHTML = html     
        });
    </script>
</html>


```

# [[Simple Storage Service|S3]]  Advanced
##         athena-s3-access-logs.sql
```sql
create database s3_access_logs_db;

CREATE EXTERNAL TABLE IF NOT EXISTS s3_access_logs_db.mybucket_logs(
         BucketOwner STRING,
         Bucket STRING,
         RequestDateTime STRING,
         RemoteIP STRING,
         Requester STRING,
         RequestID STRING,
         Operation STRING,
         Key STRING,
         RequestURI_operation STRING,
         RequestURI_key STRING,
         RequestURI_httpProtoversion STRING,
         HTTPstatus STRING,
         ErrorCode STRING,
         BytesSent BIGINT,
         ObjectSize BIGINT,
         TotalTime STRING,
         TurnAroundTime STRING,
         Referrer STRING,
         UserAgent STRING,
         VersionId STRING,
         HostId STRING,
         SigV STRING,
         CipherSuite STRING,
         AuthType STRING,
         EndPoint STRING,
         TLSVersion STRING
) 
ROW FORMAT SERDE 'org.apache.hadoop.hive.serde2.RegexSerDe'
WITH SERDEPROPERTIES (
         'serialization.format' = '1', 'input.regex' = '([^ ]*) ([^ ]*) \\[(.*?)\\] ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) \\\"([^ ]*) ([^ ]*) (- |[^ ]*)\\\" (-|[0-9]*) ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) (\"[^\"]*\") ([^ ]*)(?: ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*) ([^ ]*))?.*$' )
LOCATION 's3://target-bucket-name/prefix/';


SELECT requesturi_operation, httpstatus, count(*) FROM "s3_access_logs_db"."mybucket_logs" 
GROUP BY requesturi_operation, httpstatus;

SELECT * FROM "s3_access_logs_db"."mybucket_logs"
where httpstatus='403';
```
##         mfa-delete.sh
```bash
# generate root access keys
aws configure --profile root-mfa-delete-demo

# enable mfa delete
aws s3api put-bucket-versioning --bucket mfa-demo-stephane --versioning-configuration Status=Enabled,MFADelete=Enabled --mfa "arn-of-mfa-device mfa-code" --profile root-mfa-delete-demo

# disable mfa delete
aws s3api put-bucket-versioning --bucket mfa-demo-stephane --versioning-configuration Status=Enabled,MFADelete=Disabled --mfa "arn-of-mfa-device mfa-code" --profile root-mfa-delete-demo

# delete the root credentials in the IAM console!!!
```


##          pre-signed-url.sh
```bash


# do not forget to region parameter! (make sure it's the proper region you're choosing)
aws s3 presign s3://mybucket/myobject --region my-region

# add a custom expiration time
aws s3 presign s3://mybucket/myobject  --expires-in 300 --region my-region


# IF YOU ARE GETTING ISSUES 

# set the proper signature version in order not to get issues when generating URLs for encrypted files
aws configure set default.s3.signature_version s3v4

```

# [[Simple Queue Service|SQS]]
##         sqs.sh
```bash
# get CLI help
aws sqs help

# list queues and specify the region
aws sqs list-queues --region us-east-1

# send a message
aws sqs send-message help
aws sqs send-message --queue-url https://queue.amazonaws.com/387124123361/MyFirstQueue --region us-east-1 --message-body hello-world

# receive a message
aws sqs receive-message help
aws sqs receive-message --region us-east-1  --queue-url https://queue.amazonaws.com/387124123361/MyFirstQueue --max-number-of-messages 10 --visibility-timeout 30 --wait-time-seconds 20

# delete a message
aws sqs delete-message help
aws sqs receive-message --region us-east-1  --queue-url https://queue.amazonaws.com/387124123361/MyFirstQueue --max-number-of-messages 10 --visibility-timeout 30 --wait-time-seconds 20
aws sqs delete-message --receipt-handle AQEBB+moMioWDaeaCZguaiMPXEqDe6n4JlGiUj/T0yUCLEKkL/tT1+68xyiZMe/ip7HBvgzSZJ6Gys8CCY8QO5qPypqZ9HSKdhl6sluJVl90x1igUHwz0gSEq/UbiLB8tNvFOKF90Dj4aH87mW3K7LLNUtv839z2Uu1Aeqd4kQDVB7SSqPzqCeaYFcLGquz+XIvT69vTAYP5HIsIjmwECx0faEiQF2JZ/KiVHq5n/ZEcG5UbIPMFmP+bg1n4ql8+2dUK+6G+gnIkMRPraZ4aweT9vUZmD5AXHDU5lnJBJNKj1QGuTbxtCjp/pzJvsul/uwsspUUWdRGP92ZpTlTDTL+WiJft3E9AUdqVhksc8NhExYDpdebWEqx43SbvzJMyJlrC --queue-url https://queue.amazonaws.com/387124123361/MyFirstQueue --region us-east-1
```

# SSM
##         cli.sh
```bash
# GET PARAMETERS
aws ssm get-parameters --names /my-app/dev/db-url /my-app/dev/db-password
# GET PARAMETERS WITH DECRYPTION
aws ssm get-parameters --names /my-app/dev/db-url /my-app/dev/db-password --with-decryption

# GET PARAMETERS BY PATH
aws ssm get-parameters-by-path --path /my-app/dev/
# GET PARAMETERS BY PATH RECURSIVE
aws ssm get-parameters-by-path --path /my-app/ --recursive
# GET PARAMETERS BY PATH WITH DECRYPTION
aws ssm get-parameters-by-path --path /my-app/ --recursive --with-decryption
```

##         handler.py
```python
import json
import boto3
import os

ssm = boto3.client('ssm', region_name="eu-west-3")
dev_or_prod = os.environ['DEV_OR_PROD']

def lambda_handler(event, context):
    db_url = ssm.get_parameters(Names=["/my-app/" + dev_or_prod + "/db-url"])
    print(db_url)   
    db_password = ssm.get_parameters(Names=["/my-app/" + dev_or_prod + "/db-password"], WithDecryption=True)
    print(db_password)
    return "worked!"

```


