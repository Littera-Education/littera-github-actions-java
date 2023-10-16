# littera-github-actions-java

## Overview

A centralized source of standardized patterns for building, testing and deploying Java applications at Littera. Each pipeline takes advantage of the available actions from Littera-Education/littera-github-actions.

## Pipelines

1. `development`
    * Meant for development
    * Supports modes:
        * `develop`
            1. Maven build/test/sonar
            2. Maven minor release
            3. Build & publish image
            4. Deploy to dev environment
        * `hotfix`
            1. Maven build/test/sonar
            2. Maven patch release
            3. Build & publish image
            4. Deploy to dev environment
        * `pr`
            1. Maven build/test/sonar
2. `development-snapshot`
    * Meant for rapid development
        1. Build & publish image
        2. Deploy to dev environment
3. `promotion`
    * Meant for deploying an image to an environment
        1. Deploy to specified environment