# LAB - 16

## cloud-server

### GUI Process

1. Create Elastic Beanstalk application on AWS.

2. Create .zip folder containing server files with json.package and root index/server/app file at the root of the folder.

3. Create a new environment.
    * Upload .zip folder from earlier during this step.

- [GUI Deployed Environment](http://aws-ec2-basic.eba-i49emdwe.us-east-1.elasticbeanstalk.com/)

### CLI Process

1. Create Username and groups (with needed permission) on IAM application on AWS.
    * leave auth key and secret key tab open for next step

2. In CLI: `aws configure`
    * follow prompts to enter keys from previous step
    * enter region desired
3. In CLI: `eb init`
    * follow more prompts, choosing desired environment name and language.

4. In CLI: `eb create`
    * creates environment for deployment
    * if local repo is linked to github repo; you may need to push initial commit or create a 'ebignore' file before this step.
5. In CLI: `eb open`
    * accesses server environment
    * `eb deploy` to redeploy server if there are issues or you update code

* [CLI Deployed Environment](http://aws-ec2-basic-dev.us-west-2.elasticbeanstalk.com/)
