# README: Deploying DeepSeek Model with AWS SageMaker for RAG Application

## Overview

This guide provides instructions to deploy the **DeepSeek** model as a SageMaker endpoint and integrate it into a **Retrieval-Augmented Generation (RAG)** application. The application leverages **AWS Bedrock Knowledgebase and** **OpenSearch** to facilitate information retrieval and generate contextually accurate responses.

## Prerequisites

- AWS account with appropriate permissions
- SageMaker execution role with necessary policies
- Amazon Bedrock access with permissions to invoke foundation models
- OpenSearch serverless collection with data indexed for retrieval

## AWS Region

The demo is executed in the **ap-south-1 (Mumbai)** region. If deploying in a different region, ensure to update the region name accordingly in the script before execution.

## Model Access

The following model access is required:

### Embedding Model

- **Model Name:** Titan Embedding Text V2
- **Model ID:** `amazon.titan-embed-text-v2:0`

Ensure that the model is accessible via Amazon Bedrock before proceeding.

## SageMaker Infrastructure

### Notebook Instance

- **Instance Type:** `ml.t3.medium`
- **Purpose:** To execute the deployment script and initiate the SageMaker endpoint.

### Endpoint Instance

- **Instance Type:** `ml.g6.12xlarge`
- **Purpose:** Hosting the DeepSeek model to serve inference requests.

## Deployment Steps

Refer the deepseek_deployment.ipynb file for the step by step instructions.
