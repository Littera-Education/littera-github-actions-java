# littera-github-actions-java

## Overview

A centralized source of standardized patterns for building, testing and deploying Java applications at Littera. Each pipeline takes advantage of the available actions from Littera-Education/littera-github-actions.

## Pipelines

1. `development-pipeline`
    1. Maven build/test/sonar
    2. Maven minor release
    3. Build & publish image
    4. Deploy to dev environment
1. `hotfix-pipeline`
    1. Maven build/test/sonar
    2. Maven patch release
    3. Build & publish image
    4. Deploy to dev environment
1. `pr-pipeline`.
    1. Maven build/test/sonar
1. `snapshot-pipeline`
    1. Build & publish image
    2. Deploy to dev environment
1. `promotion-pipeline`
    1. Deploy to specified environment
