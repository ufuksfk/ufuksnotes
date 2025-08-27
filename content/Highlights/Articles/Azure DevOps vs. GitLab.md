---
draft: true
description:
socialDescription:
title: Azure DevOps vs. GitLab
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Chelsea Brown]]
url: https://www.praktikgroup.com/azure-devops-vs-gitlab/

last highlighted date: [[2024-04#03]]

## Highlights
- When it comes to actually creating a pipeline, it is important to consider to the time cost of starting up. Azure DevOps has a [YAML pipeline editor](https://learn.microsoft.com/en-us/azure/devops/pipelines/get-started/yaml-pipeline-editor?view=azure-devops) that makes it much easier to create and edit the pipelines. While GitLab also has a [Pipeline Wizard](https://docs.gitlab.com/ee/development/cicd/pipeline_wizard.html), it expects you to create and maintain a YAML template as code. Conversely, the Azure DevOps wizard doesn’t require you to write any YAML. Furthermore, GitLab doesn’t provide a visual editor for build and release orchestration like Azure DevOps. This can serve as an impedance for certain teams.
    - Note: cicd pipeline
- users must pay a monthly or annual fee that can range from $29 to $99 per user per month. This is compared to the $6 per user per month for Azure DevOps Services
    - Note: price
- If your ecosystem already has several Microsoft tools, Azure DevOps may be a better choice for your CI/CD needs. Additionally, it is customizable and integrates with other, third-party tools through plugins in the [Visual Studio Marketplace](https://marketplace.visualstudio.com/azuredevops/). Conversely, GitLab focuses more on using its own native tools and does not provide a marketplace for CI/CD plugins. This may mean an additional time cost of having to learn a new tool instead of being able to use whatever tool works best for you
    - Note: ecosystem
