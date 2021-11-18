# Terraform AWS Elastic Beanstalk Docker

Terraform script to setup AWS Elastic Beanstalk with a load-balanced Docker app

## What this script does

* Create an Elastic Beanstalk Application and environment.
* Setup the EB environment with Docker, an Elastic Loadbalancer and forward port from HTTP / HTTPS to the specified instance port.
* (Optionnal) Create a Route53 Alias to link your domain to the EB domain name
* (Optionnal) Create a Cloudfront distribution on top of your Elastic Beanstalk environment

## Customize

Many options are available through variables. Feel free to look into `variables.tf` inside each module to see all parameters you can setup.

## Terraform related documentation

* Elastic Beanstalk Application: https://www.terraform.io/docs/providers/aws/r/elastic_beanstalk_application.html
* Elastic Beanstalk Environment: https://www.terraform.io/docs/providers/aws/r/elastic_beanstalk_environment.html
* CloudFront: https://www.terraform.io/docs/providers/aws/r/cloudfront_distribution.html
* Route53: https://www.terraform.io/docs/providers/aws/d/route53_zone.html