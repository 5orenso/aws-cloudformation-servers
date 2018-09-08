# AWS Base setup with Cloudformation

An AWS Server setup from scratch with Cloudformation.

This is your server setup for your EC2 servers, server role, ELB (Elastic Load Balancer), Launch configuration and autoscaling group.

With this setup your are ready to run from 1 to many thousands of servers, all depending of your requirements. All is done with auto scaling and automatic error handling. If one of your servers goes offline, another with take it's place.

With this setup your also ready for continuous deployment of software. I use this all the time and deploy all from 1 to 20 versions every day.

### Initial setup

__This should only be run once!__

```bash
# Create the base server
$ bash ./bin/create-stack.sh --template servers
```


### Update stack

After every change you can run this command to update the stack.

```bash
# Update the base server setup.
$ bash ./bin/create-stack.sh --template servers --update-stack
```



## Other Resources

* [AWS Basic setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-base)
* [AWS Server setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-servers)
* [AWS Lambda boilerplate](https://github.com/5orenso/aws-lambda-boilerplate)
* [Automated AWS Lambda update](https://github.com/5orenso/aws-lambda-autodeploy-lambda)
* [AWS API Gateway setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-api-gateway)
* [AWS IoT setup with Cloudformation](https://github.com/5orenso/aws-cloudformation-iot)
