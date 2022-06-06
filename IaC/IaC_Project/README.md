### LINK
newka-WebAp-1PPWLAZTI6VZF-1618774011.us-east-1.elb.amazonaws.com


### Project Title - Deploy a high-availability web app using CloudFormation

#### final-project-starter.yml
Students have to write the CloudFormation code using this YAML template for building the cloud infrastructure, as required for the project. 

#### server-parameters.json
Students may use a JSON file for increasing the generic nature of the YAML code. For example, the JSON file contains a "ParameterKey" as "EnvironmentName" and "ParameterValue" as "UdacityProject". 

In YAML code, the `${EnvironmentName}` would be substituted with `Project` accordingly.

### To Run

1. Login to AWS, set IAM role and download key

2. Configure AWS in CLI and name profile

3. Set parameters in infra-params.json to choice

4. Run ./create.sh <projectname> infra-arch.yml infra-params.json --profile <profilename>

5. Check resources on AWS...

### To Delete stack
Run: aws cloudformation delete-stack --stack-name <projectname> --profile <profilename>

## To Update Resources
Run ./update.sh <projectname> infra-arch.yml infra-params.json --profile <profilename>