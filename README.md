# MLOps Capstone

<!-- TOC ignore:true -->
## Table of Contents
<!-- TOC -->

- [MLOps Capstone](#mlops-capstone)
    - [mlops capstone plan](#mlops-capstone-plan)
    - [Problem Statement](#problem-statement)
    - [Insights from EDA](#insights-from-eda)
    - [TEST IN DIFFERENT VENVS](#test-in-different-venvs)
    - [References](#references)
        - [All about the README](#all-about-the-readme)

<!-- /TOC -->

## mlops capstone plan

1. what problem do I want to solve?
1. search & shortlist dataset
1. work out problem statement
1. setup environment
   - pre-commit
   - linting
   - formatting
   - make
1. prelim EDA
1. prelim modeling
1. experiment with mlflow
1. unit test with pytest
1. prelim deploy: create POC with prelim predictions data
   - docker image to docker hub
   - localstack mock setup
   - UI app: Streamlit / Mesop(?)
1. integration test with localstack
1. setup IaC with terraform
1. orchestrate with mage
1. monitor with evidently
1. rinse & repeat, iterate 5-12

## Motivation



## Problem Statement

How has class size change since I was in school? 
Has the Pupil:Teacher ratio seen any improvement?
How does the population rate of change determine 
- how many teachers, 
- in how many schools,
- expenditure predicted amount,
we need in a five year span?

## Installation

1. Ensure script has correct permissions to run in terminal

```bash
chmod +x ./src/start.sh
```

2. Docker 
   1. Create a volume
   2. Create a network

```bash
docker volume create --name mlops-capstone-vol -d local
docker network create pg-network
```


## Insights from EDA


## TEST IN DIFFERENT VENVS

```bash
pixi shell -e py39 # Activate the py39 environment
pixi run python your_script.py # Run your code using Python 3.9
exit # Deactivate the environment

pixi shell -e dev # Activate the dev environment (similar steps)
pixi run python your_script.py
exit
```

## References

### All about the README

- https://docs.readme.com/main/docs/intro-to-readme
- https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
- vs code extensions:
  - Auto Markdown TOC

