Deploying:

Create the network stack:
aws cloudformation create-stack --stack-name UdagramNetworkStack --template-body file://udagram-network-cfn.yml --parameters file://udagram-network-params.json --region=us-west-2 

Create the servers stack:
aws cloudformation create-stack --stack-name UdagramServersStack --template-body file://udagram-servers.yml --parameters file://udagram-servers-params.json --capabilities CAPABILITY_NAMED_IAM

URl to test the application:
http://udagr-webap-1k80ubohv776i-448728279.us-west-2.elb.amazonaws.com/


