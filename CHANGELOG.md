# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

--------
# [Unity Release 23.2] - 2023-06-30

- unity-cs : https://github.com/unity-sds/unity-cs/releases/tag/23.2
- unity-cs-infra : https://github.com/unity-sds/unity-cs-infra/releases/tag/0.1.1
- unity-cs-security : https://github.com/unity-sds/unity-cs-security/releases/tag/0.1.1
- unity-cs-manager : https://github.com/unity-sds/unity-cs-manager/releases/tag/0.1.27
- unity-management-console :  https://github.com/unity-sds/unity-management-console/releases/tag/0.2.11
- unity-cs-action : https://github.com/unity-sds/unity-cs-action/releases/tag/1.0.2

## Features:
- FEATURE:  `Nightly Deployment`
- FEATURE:  `Unity SIPS Test Venue`
    - [unity-cs #196] Cognito User Groups Necessary for Unity-Sips-Test deployment
        - https://github.com/unity-sds/unity-cs-infra/tree/main/terraform-shared-services-cognito_module
    - [unity-cs #197] Cognito Users Necessary for Unity-Sips-Test deployment
    - [unity-cs #198] Shared Services (Unity-Test) authorization controls for Unity-Sips-Test access
        - https://github.com/unity-sds/unity-cs-infra/tree/main/terraform-shared-services-api-gateway_module
        - https://github.com/unity-sds/unity-cs-infra/tree/main/terraform-shared-services-api-gateway-updater_module    
    - [unity-cs #201] Automate Project Account (Unity-Sips-Test) Auth Lambda Deployment
        - https://github.com/unity-sds/unity-cs-auth-lambda
        - https://github.com/unity-sds/unity-cs-infra/tree/main/terraform-project-api-gateway_module
          
- FEATURE:  `Venue Costs`


--------
# [Unity Release 23.1] - 2023-04-07

- unity-cs : https://github.com/unity-sds/unity-cs/releases/tag/23.1
- unity-cs-infra : https://github.com/unity-sds/unity-cs-infra/releases/tag/0.1.0
- unity-cs-security : https://github.com/unity-sds/unity-cs-security/releases/tag/0.1.0
- unity-cs-manager : https://github.com/unity-sds/unity-cs-manager/releases/tag/0.1.26-Alpha
- unity-control-plan :  https://github.com/unity-sds/unity-control-plane/releases/tag/0.1.12-Alpha
- unity-cs-action : https://github.com/unity-sds/unity-cs-action/releases/tag/v1.0.1

## Epics:
- EPIC: `u-ads-jupyter-security`
    - [unity-cs #129] Custom JupyterHub Authenticator to pass Cognito tokens from JupyterHub to JupyterLab
      - https://github.com/unity-sds/unity-ads-deployment/pull/109/files
    - [unity-cs #122] Reusable python function to obtain and refresh Cognito tokens in Jupyter Notebooks
      - https://github.com/unity-sds/unity-cs-security/tree/main/code_samples/jupyter/get_and_refresh_tokens
    - [unity-cs #120, unity-cs #123] Reusable python function to obtain and refresh temporary AWS credentials in Jupyter Notebooks
      - https://github.com/unity-sds/unity-cs-security/tree/main/code_samples/jupyter/identity_pool_aws_creds
    - [unity-cs #51] Documentation and working example of how security for a user logging into Jupyterhub would work
      - Steps to integrate Amazon Cognito authentication with JupyterHub in the following wiki page.
        https://github.com/unity-sds/unity-cs/wiki/Amazon-Cognito-Authentication-with-JupyterHub
      - Approaches to get JWT Token in command line in the following wiki page. These approaches can be used in a Jupyter Notebook too.
        https://github.com/unity-sds/unity-cs/wiki/Getting-Cognito-JWT-Tokens-in-Command-Line
    - [unity-cs #74] Working example for Jupyter Notebook users to access the protected WPS-T endpoints
      - https://github.com/unity-sds/unity-cs/wiki/Accessing-Secured-REST-API-Endpoints-from-Jupyter-Notebook
- EPIC: `api-reachability-and-routing`
    - [unity-cs #116, unity-cs #114, unity-cs #57] Implemented terraform to deploy the API Gateway and update integration points through stage variables
      - https://github.com/unity-sds/unity-cs/tree/api-gateway-terraform/terraform/terraform-api-gateway
    - [unity-cs #104, unity-cs #56] API Gateway Lambda Authorizer to accept jwt access tokens of multiple client IDs and authorize requests based on Cognito user groups
      - https://github.com/unity-sds/unity-cs-security/tree/main/code_samples/api-gateway-common-lambda-authorizer-function
    - [unity-cs #189] Update API GW SSM Parameters when deploying API GW through terraform
      - Added ssm parameter resources to API GW terraform for services to use when modifying the API GW Rest API.
        https://github.com/unity-sds/unity-cs-infra/blob/0cdaeb18ad85dd1f19aab75ac8d198cd0efec5c1/terraform-project-api-gateway_module/main.tf#L11
- EPIC: `basic-deployment-docs`
  - Basic SDLC and Deployment diagram can be found here:  https://app.gitbook.com/o/xZRqGQeQXJ0RP4VMj7Lq/s/UMIRhLdbRQTvMWop8Il9/developer-docs/common-services/quick-start
  - Resource Tagging Documentation:  https://unity-sds.gitbook.io/docs/developer-docs/common-services/docs/users-guide/deployment/unity-aws-resource-tagging-conventions
- EPIC: `deployment-venue-support`
  - Tom to fill in details  

------------

--------
# [Unity Prototype 0.2] - 2022-07-28

- unity-cs : https://github.com/unity-sds/unity-cs/releases/tag/unity-prototype-0.2
- unity-security : https://github.com/unity-sds/unity-cs-security/releases/tag/unity-prototype-0.2 
- unity-cs-infra : https://github.com/unity-sds/unity-cs-infra/releases/tag/unity-prototype-0.2
- unity-cs-terraform-transformer : https://github.com/unity-sds/unity-cs-terraform-transformer/releases/tag/unity-prototype-0.2
- unity-cs-deployment-catalog : https://github.com/unity-sds/unity-cs-deployment-catalog/releases/tag/unity-prototype-0.2
- gitbook Documentation : https://unity-sds.gitbook.io/docs/developer-docs/common-services (this is still a WIP, but as of 7/28 represents the 0.2 release..)


- EPIC: `deployment-venue-support`
  - coming soon...

---------------
## [0.1.0] - 2022-04-20

### Added 

- 
-
-
