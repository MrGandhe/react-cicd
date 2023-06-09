# React App Deployment on Cloudfront 

<h1 align="center"> Virtuecloud </h1> <br>
<p align="center">
  <a href="https://virtuecloud.io/">
    <img alt="Virtuecloud" title="Virtuecloud" src="https://virtuecloud.io/assets/images/VitueCloud_Logo.png" width="450">
  </a>
</p>

## Table of Contents

- [Introduction](#introduction)
- [Feature](#Feature)
- [Inputs](#Inputs)
- [Workflow](#Workflow) 

# Introduction

This repository contains the source code to create a CI/CD pipeline for a React application in AWS. The pipeline pulls the source code from GitHub and run tests against the application to build it before deploying it to an S3 bucket for static site hosting. The site will then be distributed using CloudFront which will point to the S3 bucket.

# Feature

We have used the composite actions here:
   * To build the react app
   * To deploy the build to S3 Bucket
   * To invalidate cache 

 
# Inputs

|Name              |Description|Type|Default|
|------------------|-----------|-------|-------|
|Bucket    |Name of your bucket |string |""|
|Cloudfront_distribution_ID  |Distribution ID of Cloudfront Distribution created  |string |""|

# Workflow

## Step1:
Firstly, we defined environment to run the job.
## Step3:
Configured AWS Credentials
## Step4:
Set up the node Environment to run app

