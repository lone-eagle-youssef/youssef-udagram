# Pipeline Process

## Overview

Through Github, this application is connected to CircleCI. Any modifications to the master branch will trigger a series of deployment-related actions in CircleCI.
The steps are in this order:

- Spin up environment
- Preparing environment variables
- Install NodeJS node
- Install NPM
- Checkout code
- Setup AWS CLI - latest
- Configure AWS Access Key ID
- Setting Up Elastic Beanstalk CLI
- Install Back-End Dependencies
- Build Back-End
- Install Front-End Dependencies
- Build Front-End
- Deploy Backend
- Deploy Frontend

### Diagram

[](pipline.md)
