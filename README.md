# Basic Amazon Lambda using Serverless

# Installation

> npm init --yes
> npm install serverless

Example to set up the Amazon Web Services Key and Secret usign Command
> npx serverless config credentials --provider aws --key AKIAIOSFODNN7EXAMPLE --secret wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY

To see other ways as AWS-Cli see:
https://github.com/serverless/serverless/blob/HEAD/docs/providers/aws/guide/credentials.md

Create a NodeJS Serverless
> serverless create --template aws-nodejs --path hello-world
> cd hello-world

# Test on your Local Machine
> npx serverless invoke local -f hello -l

This will call your handle.js the module.exports.hello function

# Deploy

Deploy Service
Service is the configuration of the Amazon Lambda contained in the hello-world/serverless.yml

> serverless deploy -v

Deploy function
Deploy the .js function hello-world/handler.js
> serverless deploy function -f hello



