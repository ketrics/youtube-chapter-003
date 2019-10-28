## Splitted stacks

### CloudFormation commands

#### Create or Update
    aws cloudformation <create-update>-stack --stack-name <StackName> \
    --template-body file://$PWD/template.yml \
    --parameters file://$PWD/parameters.json

#### Delete
    aws cloudformation delete-stack --stack-name <StackName>


### Deploy networking stack to the cloud
    aws cloudformation create-stack \
    --stack-name ketricslabs-network \
    --template-body file://$PWD/network.yml
    --parameters file://$PWD/parameters.json

### Deploy ec2 stack to the cloud
    aws cloudformation create-stack \
    --stack-name ketricslabs-ec2 \
    --template-body file://$PWD/ec2.yml
    --parameters file://$PWD/parameters.json