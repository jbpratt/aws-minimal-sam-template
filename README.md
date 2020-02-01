AWS Minimal SAM Template
========================

Personal template for a minimal Python3.8 Lambda with an existing role

-	Install the [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html) to create a project

Setup
-----

```
~ >sam init
Which template source would you like to use?
	1 - AWS Quick Start Templates
	2 - Custom Template Location
Choice: 2

Template location (git, mercurial, http(s), zip, path): https://github.com/jbpratt78/aws-sam-minimal-template.git
```

-	Install [pre-commit](https://pre-commit.com/) and run `pre-commit install` to set up Git hooks.
-	Add dependencies to src/requirements.txt

Build and Deploy
----------------

Modify the `template.yaml` as needed, setting the

```
sam build --use-container
sam deploy --guided
```
