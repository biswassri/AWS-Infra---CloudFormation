# infrastructure
This Repo into create the Infrastructure layer

# Creating the Stack with Cloud formation

```
aws cloudformation create-stack --stack-name myteststack 
--template-body file://vpc.json 
--parameters ParameterKey=Name,ParameterValue=REDACTED ParameterKey=cidrBlock,ParameterValue= REDACTED ParameterKey=region,ParameterValue=REDACTED
```
# Delete the Cloudformation Stack

```
aws cloudformation delete-stack --stack-name myteststack

```

# Wait for the Cloudformation Stack to get deleted 

```
aws cloudformation wait stack-delete-complete --stack-name myteststack
```
