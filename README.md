# OWASP Serverless Top 10 as code

Demo repository for the OWASP APAC 2022 Conference

## Introduction

This repository includes a sample DevSecOps Github Action workflow that includes secret detection, DAST and SCA scanners.

## Sample serverless app

* The sample app for the demo is a serverless application. You can deploy it using Serverless Framework. 
* You can install the Serverless framework CLI using `npm install -g serverless`. 
* To test the application locally, a `docker-compose` file has been added with `localstack`. 
* To deploy the app to localstack use the following command `sls deploy --stage local`.

## DevSecOps workflow

The security workflow includes the following security controls:
* Secret Detection using `Gitleaks`
* DAST using `ZAP`
* SCA using OWASP `dependency-check`
* Github MFA checker
