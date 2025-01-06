# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

--------
# [Unity Release 24.2 - 24.4] - 2025-01-06

- unity-cs : https://github.com/unity-sds/unity-cs/releases/tag/24.4
- unity-cs-infra : https://github.com/unity-sds/unity-cs-infra/releases/tag/TBD
- unity-cs-security : https://github.com/unity-sds/unity-cs-security/releases/tag/TBD
- unity-cs-manager : https://github.com/unity-sds/unity-cs-manager/releases/tag/TBD
- unity-management-console :  https://github.com/unity-sds/unity-management-console/releases/tag/TBD
- unity-marketplace : https://github.com/unity-sds/unity-marketplace/releases/tag/TBD

## 24.2:
- BUG FIXES AND IMPROVEMENTS:
    - [unity-cs #](https://github.com/unity-sds/unity-cs-infra/issues/17)  Set endpoints for a venue in a configuration	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/305)  Investigate SSL cert via Shared Services CloudFront	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/315)  Shared Services HTTPD proxy Work (CS)	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/323)  httpd terraform module finalization	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/352)  Integrate HTTPD into the Reference Application
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/354)  Fix HTTPS/HTTP issue with HTTPD authentication of Management Console	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/355)  Enable HTTPS in Management Console	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/358)  Track Down and delete mystery untagged resource	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/365)  Make MC version flexible in CF template	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/366)  Management Console 24.2 Features	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/367)  Implement lambda in Venue account to periodically gather health status	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/370)  Create SSM parameter for monitoring S3 bucket name	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/372)  Update documentation to include necessary Cognito roles/users	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/373)  Add SSM parameter that specifies shared services account in venue creation process	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/374)  Venue Creation scripts would copy shared services health check SSM params into venue	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/376)  Add SSM Parameter that identifies the cognito domain assigned to the respective user pool of a given venue	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/397)  Ensure Cloudfront Distributions have a default Root Object	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/377)  Clean up Unity-Test Cognito User Pools	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/379)  Update SSM Documentation and Guidelines to support project/venue specific params	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/375)  Add SSM Parameter that identifies the shared services CloudFront distribution for a given venue	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/380)  Create Monitoring S3 bucket upon Management Console deployment	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/381)  Create Backend API to Serve Health Statuses of Deployed services in a proj/venue	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/383)  Fix the broken Management Console Deployment due to GH Token	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/385)  Mock Up Initiators Configuration Template for Review	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/388)  Determine how DAPA Client ID SSM param gets populated in Shared Services	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/389)  Determine how DAPA API URL SSM param gets populated in Shared Services	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/391)  Change S3 Bucket SSM param name and value to something generic.	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/392)  Remove Dependency of Management Console on /unity/core/project|venue SSM param	
    - [unity-cs #](https://github.com/unity-sds/unity-on-demand/issues/37)  Setup Initiators Github repos	
    - [unity-cs #](https://github.com/unity-sds/unity-on-demand/issues/38)  Create Schema that Validates Initiators Configuration	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/393)  Build out Lambda repository and build actions	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/398)  Properly namespace the Management Console URL SSM parameter	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/399)  Further cleanup of /unity/core/venue|project SSM Needed	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/400)  Create a common SSM param for /unity/cs/account/network/certificate-arn	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/401)  move proxy lambda SSM param to venue/project namespace	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/403)  HTTPD configuration Management Improvements	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/404)  Create EC2 HTTPD Dev Server in Unity-venue-dev	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/405)  Setup Authentication on shared services HTTPD	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/406)  Create Venue JupyterHub HTTPD config/rewrite rules	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/409)  Remove deprecated API GW code	
    - [unity-cs #](https://github.com/unity-sds/unity-cs/issues/410)  Determine how to access Cognito user pool in SS account from Venue account	
    - [unity-cs #414](https://github.com/unity-sds/unity-cs/issues/414)  Find a solution to support multiple httpd callback URLs	

## 24.3:
- BUG FIXES AND IMPROVEMENTS:
    - Provide ability for U-ADS to use HTTPD with Jupyterhub	https://github.com/unity-sds/unity-project-management/issues/170
    - Get navbar into the Marketplace (needs httpd)	https://github.com/unity-sds/unity-ui/issues/30
    - Unity-Prod Shared Services common auth: Cognito Groups, Users (CS)	https://github.com/unity-sds/unity-cs/issues/313
    - Rework SPS Marketplace installation to use EKS/httpd	https://github.com/unity-sds/unity-cs/issues/351
    - Create Backend API method and API GW route to Serve Landing pages of Deployed services in a proj/venue	https://github.com/unity-sds/unity-cs/issues/382
    - Populate the Shared Services DAPA Client ID SSM param in a Venue Deployment	https://github.com/unity-sds/unity-cs/issues/386
    - Populate the Shared Services DAPA API URL in a Venue Deployment	https://github.com/unity-sds/unity-cs/issues/387
    - Add common SSM param to venue for the AWS region	https://github.com/unity-sds/unity-cs/issues/407
    - Make API Gateway name dynamic, not hardcoded to SampleProject	https://github.com/unity-sds/unity-cs/issues/408
    - Rework Dev Proxy Topology & Configuration	https://github.com/unity-sds/unity-cs/issues/416
    - SSM configuration modification for MC deployments	https://github.com/unity-sds/unity-cs/issues/417
    - Enable versioning on shared venue buckets	https://github.com/unity-sds/unity-cs/issues/418
    - Landing URL, Service Name & Final Testing of Monitoring Feature	https://github.com/unity-sds/unity-cs/issues/423
    - Make deletion/creation of S3 bucket a flag for MC bootstrap	https://github.com/unity-sds/unity-cs/issues/424
    - Look into Namespacing ECS cluster tasks with venue & project	https://github.com/unity-sds/unity-cs/issues/425
    - Remove Unecessary ports in internal ALB	https://github.com/unity-sds/unity-cs/issues/426
    - Add IAM role create service linked role command to venue role script	https://github.com/unity-sds/unity-cs/issues/427
    - Initiators: Research and prototype CMR trigger options (POLLING)	https://github.com/unity-sds/unity-cs/issues/437
    - Initiators: High-level logging & Traceability of initiators/triggers events	https://github.com/unity-sds/unity-cs/issues/439
    - Management console log groups should be unique to project and venue and Log Retention Time should be set to 30 days	https://github.com/unity-sds/unity-cs/issues/441
    - Update Venue httpd config to support management rewrite rule	https://github.com/unity-sds/unity-cs/issues/442
    - Move the cloudformation cfn repo code into a sub-directory of unity-cs-infra repo	https://github.com/unity-sds/unity-cs/issues/443
    - Lock down MC EC2 Bastion hosts outgoing ports to only 80, 8080, and 443, and put in private subnet	https://github.com/unity-sds/unity-cs/issues/444
    - Update mono repo docs to make final health check	https://github.com/unity-sds/unity-cs/issues/445
    - Add logging for cloudformation actions during MC deploy	https://github.com/unity-sds/unity-cs/issues/446
    - Add/improve logging related to the destruction of MC	https://github.com/unity-sds/unity-cs/issues/447
    - Create subnet SSM params in shared services account(s)	https://github.com/unity-sds/unity-cs/issues/448
    - destroy.sh script should work first time on bastion host	https://github.com/unity-sds/unity-cs/issues/449
    - Document template httpd configuration structure for shared services	https://github.com/unity-sds/unity-cs/issues/450
    - Do Rolling Check on Smoke Test after deploy	https://github.com/unity-sds/unity-cs/issues/453
    - Make health check API get "latest" file explicitly	https://github.com/unity-sds/unity-cs/issues/454
    - Add Lifecycle rule to cleanup S3 bucket files in Venue	https://github.com/unity-sds/unity-cs/issues/456
    - Archive the cfn repository	https://github.com/unity-sds/unity-cs/issues/457
    - Move MC health check SSM endpoints to be the SS proxy URL	https://github.com/unity-sds/unity-cs/issues/458
    - Update destroy.sh and docs about bucket delete / default behavior	https://github.com/unity-sds/unity-cs/issues/461
    - MC:  Uninstall button should be Removed	https://github.com/unity-sds/unity-cs/issues/462
    - Management Console bootstrap.go Code Understanding and Improvement	https://github.com/unity-sds/unity-cs/issues/464
    - Research & Fix Cookies Piling Up Issue	https://github.com/unity-sds/unity-cs/issues/466
    - Deploy Network Stack and MC to emit-dev Venue	https://github.com/unity-sds/unity-cs/issues/467
    - Create command-line arguments that control what things get installed in the Management Console	https://github.com/unity-sds/unity-cs/issues/468
    - Optimize Unnecessary sleeps in the MC Go Code during deployment	https://github.com/unity-sds/unity-cs/issues/469
    - Config File Driven Deployment Versions	https://github.com/unity-sds/unity-cs/issues/470

## 24.4:
- BUG FIXES AND IMPROVEMENTS:
    - U-DS Data Bucket in marketplace	https://github.com/unity-sds/unity-project-management/issues/144
    - Create JupyterHub unity-marketplace metadata.json	https://github.com/unity-sds/unity-ads/issues/1
    - Create s3 gateways in the Proj/Venue VPC to provide non-NAT access to AWS S3 resources.	https://github.com/unity-sds/unity-project-management/issues/209
    - Airflow integration into Unity Marketplace	https://github.com/unity-sds/unity-project-management/issues/210
    - Implement shared services to dev proxy for SPS airflow endpoints	https://github.com/unity-sds/unity-cs/issues/429
    - Integrate MC HealthCheck API with Venue API Gateway	https://github.com/unity-sds/unity-cs/issues/459
    - Improve MC UI branch field	https://github.com/unity-sds/unity-cs/issues/473
    - Always show what the injected variables are in the MC	https://github.com/unity-sds/unity-cs/issues/474
    - MMGIS integration into Unity Marketplace	https://github.com/unity-sds/unity-project-management/issues/211
    - [Feature] Put navbar UI into the Marketplace	https://github.com/unity-sds/unity-sds-portal/issues/9
    - Deploy navbar/health-dashboard/mgmt-console as a base bootstrap-deploy	https://github.com/unity-sds/unity-cs/issues/483
    - Remove project and venue variables from the u-ds marketplace json	https://github.com/unity-sds/unity-cs/issues/486
    - Demo the deployment of U-DS bucket via MC in a Unity Team meeting	https://github.com/unity-sds/unity-cs/issues/487
    - JupyterHub Integration into Unity Marketplace: Understand and Test Manual deployment as-is	https://github.com/unity-sds/unity-cs/issues/489
    - Create s3 gateways in the Proj/Venue VPC to provide non-NAT access to AWS S3 resources	https://github.com/unity-sds/unity-cs/issues/492
    - Move towards HTTP requests instead of WS API calls in Uninstall & Install actions	https://github.com/unity-sds/unity-cs/issues/494
    - Research how to properly recreated the Unity-CS_Service_Role Without Disrupting stuff	https://github.com/unity-sds/unity-cs/issues/498
    - Improve Behavior on Uninstall Apps	https://github.com/unity-sds/unity-cs/issues/502
    - Make Uninstalled Tiles Dismissable	https://github.com/unity-sds/unity-cs/issues/503
    - [Bug]: API Gateway deployments are not setting the Cognito configs in  unity-apigateway-unity-cs-common-lambda-authorizer	https://github.com/unity-sds/unity-cs/issues/500
    - Fix Issue with lifecycle rule deleting terraform state file in s3 bucket	https://github.com/unity-sds/unity-cs/issues/509
    - Fix the NLB security group to allow access from VPC Link / API Gateway in venue	https://github.com/unity-sds/unity-cs/issues/510

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
    - [unity-cs #285](https://github.com/unity-sds/unity-cs/issues/285) return error logs to webconsole is terraform fails
    - [unity-cs #317](https://github.com/unity-sds/unity-cs/issues/317) [New Feature]: Develop method to allow services to register with httpd
    - [unity-cs #363](https://github.com/unity-sds/unity-cs/issues/363) Make distinct IDs for install button in the Marketplace/Deployment web page in Management Console
    - [unity-cs #364](https://github.com/unity-sds/unity-cs/issues/364) Add text in Marketplace MC UI that displays the version numbers for deployables

- FEATURE: `Nightly Deployment`
    - [unity-cs #298](https://github.com/unity-sds/unity-cs/issues/298) Update docs on how to properly architect a Marketplace module
    - [unity-cs #322](https://github.com/unity-sds/unity-cs/issues/322) unused run.sh script
    - [unity-cs #357](https://github.com/unity-sds/unity-cs/issues/357) Fix nightly cron jobs
    - [unity-cs #359](https://github.com/unity-sds/unity-cs/issues/359) Add Parameter to run script for MC version
    - [unity-cs #360](https://github.com/unity-sds/unity-cs/issues/360) Verify that all the MC AWS resources get uninstalled
    - [unity-cs #362](https://github.com/unity-sds/unity-cs/issues/362) Installation and Testing of Management Console on Barebones Amazon Venue
      
- FEATURE:  `Production Shared Services`
    - [unity-cs #312](https://github.com/unity-sds/unity-cs/issues/312) Production API Gateway deployed (CS API Gateway)
    - [unity-cs #318](https://github.com/unity-sds/unity-cs/issues/318) Fix MIME type issues with CloudFront origin accessing MC through httpd proxy
    - [unity-cs #314](https://github.com/unity-sds/unity-cs/issues/314) Shared Services common auth deployed (CS)
    - 

- FEATURE:  `SBG Venue`
    - [unity-cs #320](https://github.com/unity-sds/unity-cs/issues/320) Venue API Gateway (CS)
    - [unity-cs #321](https://github.com/unity-sds/unity-cs/issues/321) Lambda Authorizer (CS)
 
- FEATURE:  `Unity SIPS Test Venue`
    - [unity-cs #192](https://github.com/unity-sds/unity-cs/issues/192) Ensure that U-DS Shared Services are Deployed to Unity-Test AWS Account and Accessible by SPS
    - [unity-cs #246](https://github.com/unity-sds/unity-cs/issues/246) Push-button EKS Deployment via Management Console as a Marketplace entry (Dependency from SPS)
    - [unity-cs #247](https://github.com/unity-sds/unity-cs/issues/247) Push-button API Gateway Deployment (Dependency from SPS)
 
- FEATURE:  `View Run Logs`
    - [unity-cs #75](https://github.com/unity-sds/unity-project-management/issues/75) As an operator, I want to view run logs in order to debug errors (joint UI/UX/SPS/CS ticket)
 
- NO FEATURE:
    - [unity-cs #353](https://github.com/unity-sds/unity-cs/issues/353) Add creation of U-CS_Service_Policy to Cloudformation template
    - [unity-cs #356](https://github.com/unity-sds/unity-cs/issues/356) Refresh GH token for nightlies

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
