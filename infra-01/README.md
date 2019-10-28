## Single stack

### Deploy stack to the cloud without parameters file
    aws cloudformation create-stack \
    --stack-name ketricslabs \
    --template-body file://$PWD/infra.yml


### Deploy stack to the cloud with parameters file
    aws cloudformation create-stack \
    --stack-name ketricslabs \
    --template-body file://$PWD/infra.yml \
    --parameters file://$PWD/parameters.json