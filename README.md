# CircleCI Orbs

CircleCI Orbs that make my life easier 😊 

## SDKMAN!

Setups and installs SDK with [SDKMAN!](https://sdkman.io)

[View on CircleCI](https://circleci.com/orbs/registry/orb/joshdholtz/sdkman)

```yml
orbs:
  sdkman: joshdholtz/sdkman@0.2.0
  
jobs:
  build:
    steps:
      - checkout
      - sdkman/setup-sdkman
      - sdkman/sdkman-install:
          candidate: java
          version: 8.0.265.j9-adpt
      - run: java -version
```
