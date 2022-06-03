### Project Title - Deploy a high-availability web app using CloudFormation
This project deploys a high available web app using Cloud Formation

The Load Balancer URL: http://udagr-udagr-1bn2u81gbm6qc-624874591.us-east-1.elb.amazonaws.com

The  folder contains 4 cloud formation templates

- udagraminfra.yml - This contains the Networking resources which will act as the base on where the server resources will be deployed
- udagraminfra-params.json - This declares the parameters used in the udagraminfra.yml
- udagramserver.yml - This contains the Server resources including the autoscalling group, security groups, loadbalancer, target groups, listener and the listener rule
- udagramserver-params.json - This declares the parameters used in the udagramserver.yml


The evironment architecture diagram is in the udagram Infrastructure Diagram.jpeg file

I have also created some bash scripts to help to easily deploy the templates

- create.sh - creates the cloudformation stack
- update.sh - updates a cloudformation stack
- delete.sh - deletes a cloudformation stack