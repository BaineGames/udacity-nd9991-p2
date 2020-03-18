# udacity-nd9991-p2
Udacity Cloud DevOps Engineer Project 2 - CloudFormation

## Link to See it Live for submission
http://p2-se-webap-xov7jpqircfk-1024648911.us-west-2.elb.amazonaws.com/


## Deploy Network

```
aws cloudformation create-stack --stack-name p2-network --template-body file://lesson-network.yml --parameters file://lesson-network.json --region=us-west-2
```

## Deploy Servers

```
aws cloudformation create-stack --stack-name p2-servers --template-body file://lesson-servers.yml --parameters file://lesson-servers.json --capabilities CAPABILITY_IAM CAPABILITY_NAMED_IAM CAPABILITY_AUTO_EXPAND --region=us-west-2
```
