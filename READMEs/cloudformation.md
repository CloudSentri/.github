# {{project name}}

![Review](https://gitlab.com/{{ project path }}/badges/main/pipeline.svg)

> **NOTE:** you must change the static pipeline link in the above image url for badge to work successfully and then remove this **note**

## Table of contents

- [TL;DR](#tldr)
- [Purpose](#purpose)
- [Prerequisites](#prerequisites)
- [Constraints or Conditions](#constraints-or-conditions)
- [Deployment Details](#deployment-details)
  - [CloudFormation Quick Launch](#cloudformation-quick-launch)
  - [Manual Console Configuration](#manual-console-configuration)
  - [CDK](#cdk)
  - [Automation](#automation)
- [Contribution](#contribution)

## TL;DR

{{ brief description }}

- Stack name: `{{ stack name }}`
- Deployment Account(s):
  - [ ] Management
  - [ ] Child
- Deployment Type(s):
  - [ ] Stack
  - [ ] StackSet
  - [ ] CDK
  - [ ] CLI/API
- Region(s):
  - Primary: `{{ region }}`
  - list others

## Purpose

{{ 1-3 sentence(s) of solution and what it does }}

## Prerequisites

{{ requirements for the deployment of this solution / resource }}

## Constraints or Conditions

{{ example: resources can only be deployed in specific region(s) }}

## Deployment Details

Listed here are the different deployment options for this solution.

### Require Parameters

{{ what (if any) parameters are required or do not have default values }}

1. `{{ param name}}` - description

> NOTE: Other `default` parameters may be updated of overridden via parameters file or CLI.

### CloudFormation Quick Launch

1. Login to AWS Account
2. Have this README.md open in same browser session
3. Click the `Launch Stack` button below to launch stack and supply parameters.

[![LaunchStack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://console.aws.amazon.com/cloudformation/home?region=REGION#/stacks/create/review?stackName=STACK-NAME&templateURL=https://BUCKET-NAME.s3.amazonaws.com/TEMPLATE-PATH.yml)

> **NOTE:** you must change the link params in the above image url for button to work successfully and remove this **note**

### Manual Console Configuration

When deploying manually be sure to properly name and case parameters and names:

- Upload of template file:

```sh
stackname: filename without extension
```

- S3 Object URL:

```sh
https://{{resouce bucket}}.s3.amazonaws.com/{{template object path}}.yml
```

- S3 URI

```sh
s3://{{resouce bucket}}.s3.amazonaws.com/{{template object path}}.yml
```

### CDK

Deployment via the CDK is supported and will deploy the template provided in the [cloudformation](cloudformation/) directory.

```sh
cdk deploy {{ stack-name }} --parameters myKey=myValue
```

> **NOTE:** Be sure to pass any require parameters and/or parameter overrides.

### Automation

{{ is there any automation that deploys this solution }}

## Contribution

To make changes to this project, please follow appropriate protocol to track history.

1. Fork/Clone the Project: `git clone {{repo url}}`
2. Create your Feature Branch: `git checkout -b feature/AmazingFeature`
3. Commit your Changes: `git commit -m 'Add some AmazingFeature'`
4. Push to the Branch: `git push origin feature/AmazingFeature`
5. Open a Pull Request
6. If required, request review of PR and have a second individual Pull the change

### Road Map and Open Issues

See the [open issues](../../issues) for a list of proposed features (and known issues).
