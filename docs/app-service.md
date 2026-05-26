# Enterprise Azure Infrastructure Lab - App Service Phase (PaaS)

## Objective

- Host my Todo Application in Azure App Service, and using GitHub repository to get the code packaged.
  (Due to using only Azure Student Subscription and having limitations, it can't totally host my Application but,
  I create Azure App Service and integrate it in my GitHub Repository.)

## App Service Architecture

- Separate Resource Group that only contains for Application Hosting
- Get the code in GitHub Repository
- Use B1 Basic in Service Plan
- Node 22 LTS (For better support)

## Design Decisions

- Push my code in my GitHub Repository
- Create a Web App in App Service
- Integrate my Repository to host in App Service

## Expected Learnings

- Using GitHub Repository to host a Application is way more easy
- PaaS service is a lightweight modification only

## Errors Occurred

- Can't host the website before because it's only a basic html and not using Node so the runtime is not available
- Too much create and delete app service resource due to error so it increase throttling duration
- 429 - App Service Plan Create operation is throttled
