# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

--------
# [Unity Release 24.1] - 2024-04-06

- unity-cs : https://github.com/unity-sds/unity-cs/releases/tag/24.1
- unity-cs-infra : https://github.com/unity-sds/unity-cs-infra/releases/tag/0.1.4
- unity-cs-security : https://github.com/unity-sds/unity-cs-security/releases/tag/0.1.2
- unity-cs-manager : https://github.com/unity-sds/unity-cs-manager/releases/tag/0.1.28-Alpha
- unity-management-console :  https://github.com/unity-sds/unity-management-console/releases/tag/0.4.5
- unity-marketplace : https://github.com/unity-sds/unity-marketplace/releases/tag/0.2

## Features:
- FEATURE:  `Jupyter Marketplace`
    - 
      
- FEATURE:  `Management Console`
    -     
- FEATURE:  `Marketplace Integration`
    - 

- FEATURE:  `Navbar hard-coded`
    - 
 
- FEATURE:  `Operator Test Venue`
    - 
 
- FEATURE:  `Unity SIPS Test Venue`
    - 

--------

# [Unity Release 23.3] - 2023-09-26

- unity-cs : https://github.com/unity-sds/unity-cs/releases/tag/23.3
- unity-cs-infra : https://github.com/unity-sds/unity-cs-infra/releases/tag/0.1.2
- unity-cs-security : https://github.com/unity-sds/unity-cs-security/releases/tag/0.1.1
- unity-cs-manager : https://github.com/unity-sds/unity-cs-manager/releases/tag/0.1.27-Alpha
- unity-management-console :  https://github.com/unity-sds/unity-management-console/releases/tag/0.2.17
- unity-marketplace : https://github.com/unity-sds/unity-marketplace/releases/tag/0.1

## Features:
- FEATURE:  `Jupyter Marketplace`
    - [unity-cs #254] Modify Marketplace Automation to look for Terraform files in user-supplied sub-directories (dependency from U-ADS)
      
- FEATURE:  `Management Console`
    - [unity-cs #265]Implement approach for Terraform apply for deployment in MC
    - [unity-cs #259]Implement Management Console Teardown API endpoint
    - [unity-cs #257]Switch websocket in go to an eventbus driven pipeline
    - [unity-cs #255]Migrate EKS to its own package
    - [unity-cs #250]Define interfaces and touch points for next development sprint
    - [unity-cs #249]Test suite for existing code
    - [unity-cs #220]Augment Management Console with endpoints needed by nightly/other
    - [unity-cs #211]Implement SW Deployment Teardown via S3-backed TF State
    - [unity-cs #244]Track changes in ssm param values vs config expectation
    - [unity-cs #242]Figure out how to reconnect to an install log stream if refresh is hit or connection lost
    - [unity-cs #237][New Feature]: persist installed applications in SQLite Database
    - [unity-cs #239][New Feature]: Migrate UI websocket to more of a message bus flow with handlers handing off it.
    - [unity-cs #235][New Feature]: Fix logging properly for act in management console
    - [unity-cs #234][New Feature]: CI for marketplace to create 1 combined manifest
    - [unity-cs #232][New Feature]: CI validator for marketplace
    - [unity-cs #245] Investigate Terraform managed EKS(CTL)
          
- FEATURE:  `Marketplace Integration`
    - [unity-cs #258] Integrate Project Account API GW IAC into Marketplace

- FEATURE:  `Navbar hard-coded`
    - [unity-cs #248] Need to fully define Role/Identify nomenclature (dependency from UI/UX)
 
- FEATURE:  `Operator Test Venue`
    - this feature wasn't included in this release.
 
- FEATURE:  `Unity SIPS Test Venue`
    - [unity-cs #260] Investigate Not having Thousands of API GW routes in Shared Services API GW

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
    - [unity-cs #151] Nightly Deploy & Teardown via Github Actions
    - [unity-cs #132] Nightly SSM/TF param management + flow (partially implmented, some sub-items pushed to 23.3)
    - [unity-cs #131] Implement GH Actions Teardown for EKS
    - [unity-cs #124] Integrate API Gateway script into Nightly CI Deploys
    - [unity-cs #222] Integrate Terraform bootstrap code/scripts into Management Console EC2 (partially implmented, some sub-items pushed to 23.3)
    - [unity-cs #224] Populate & Display Base SSM Params in the Management Console UI
    - 
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
    - [unity-cs #193] Confirm that Unity-Sips-Test has necessary deployment permissions #193
    - [unity-cs #200] Implement API Gateway creation scripts/terraform #200
    - [unity-cs #202] Automate Project Account (Unity-Sips-Test) SSM Deployment #202
    - [unity-cs #203] Automate Project Account (Unity-Sips-Test) EKS Deployment #203
    - [unity-cs #219] [New Feature]: Deploy software properly using act and correct commands #219
    - [unity-cs #225] Hook Front-end of Management Console up to backed deployment logic #225
    - [unity-cs #227] [New Feature]: Package workflows with management console #227
    - [unity-cs #229] [New Feature]: Let config panel look up existing ssm params to prepopulate config #229
    - [unity-cs #230] [New Feature]: look up network subnets from aws #230
    - [unity-cs #231] [New Feature]: convert messages to all protobuf #231
    - [unity-cs #233] [New Feature]: Wire up bootstrap for API gateway installation #233
    - [unity-cs #238] [New Feature]: reload config from database on app start #238
    - [unity-cs #243] Remove progress bar / detect completion and show continue button on install finish #243
          
- FEATURE:  `Venue Costs`
    - [unity-cs #98] Mechanism to query tagged resources
    - [unity-cs #96] Documentation / Guidance for Tagging
        - https://unity-sds.gitbook.io/docs/developer-docs/common-services/docs/users-guide/deployment/unity-aws-resource-tagging-conventions
    - [unity-cs #128] Apply Mandatory Tags to EKS Cluster
    - 

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
