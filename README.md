
# GitHub Actions Partner Runner Images 

**Table of Contents**

- [About](#about)
- [Available Images](#available-images)
- [Current Partner image overview](#current-partner-image-overview)
- [Image Definitions](#image-definitions)
- [Software and Image Support](#software-and-image-support)
- [How to Interact with the Repo](#how-to-interact-with-the-repo)
- [FAQs](#faqs)

## About

This repository contains the information about the VM images provided by GitHub partners which can be used on [GitHub-hosted larger runners](https://docs.github.com/en/actions/using-github-hosted-runners/using-larger-runners).

Partner images are VM images which are created by third parties which GitHub Hosted Action runner customers can use to improve particular use cases in their workflow by providing particular tools in 'one click' to work with. 

## Available Images

| Image | YAML Label | Included Software | Rollout Progress of Latest Image Release |
| --------------------|---------------------|--------------------|---------------------|
| [Ubuntu 22.04 by Arm Limited]]() | custom in larger runners| [Ubuntu 22.04 Inventory](https://arm-software.github.io/AVH/main/infrastructure/html/avh_gh_inventory.html ) | In Beta (Public)
| [ARM-Partner-AVH](https://resources.github.com/arm-gihub-actions-beta/) | custom in larger runners| [AVH Inventory](https://arm-software.github.io/AVH/main/infrastructure/html/avh_gh_inventory.html ) | In Beta (Private)

## Current Partner image overview 

### [ARM AVH Image (Beta) ](https://arm-software.github.io/AVH/main/infrastructure/html/avh_gh.html)
Arm Virtual Hardware (AVH) images contain ready-to-use Arm Cortex-M simulation models and Compiler toolchains for native use with GitHub Actions. This image is for customers who have ARM edge IoT use cases and workloads that they would like to build and test through GitHub Actions. The types of customers will be those working in industries like Medical devices, Agriculture, Consumer electronics, automotive, etc. 

## Image Definitions

### Beta

The purpose of a Beta is to collect feedback on an image before it is released to GA. 
The goal of a Beta is to identify and fix any potential issues that exist on that image. 
Images are updated on a cadence owned by the third party who provided the image, please see the image information above. 
Any workflows that run on a beta image do not fall under the customer [SLA](https://github.com/customer-terms/github-online-services-sla) in place for Actions.
Customers choosing to use Beta images are encouraged to provide feedback in the [partner-runner-images repo](https://github.com/actions/partner-runner-images/issues/new/choose) by creating an issue. 
A Beta may take on different availability, i.e. public vs private.

### GA

A GA (General Availability) image has been through a Beta period and is deemed ready for general use. Images are updated on a weekly cadence. In order to be moved to
GA the image must meet the following criteria:

1. Has been through a Beta period (public or private)
2. Most major software we install on the image has a compatible version for the underlying OS
3. All major bugs reported during the Beta period have been addressed

Any workflows that run on a partner image do not fall under the customer [SLA](https://github.com/customer-terms/github-online-services-sla) as GitHub cannot commit to the partner updating the image within these timeframes. 

## Software and Image Support

### Support Policy

- Updates to each image are owned and managed by the partner providing the image, not GitHub
- GitHub makes no warranties or guarantees for the images or their contents 
- Each partner image will have a different term of support depending on the partner, partner support links can be found below


| Partner  | Image | Support Link | 
|-----------|-----------|-----------------------|
| Arm Limited, Inc.| [Ubuntu 22.04 by Arm Limited]()| [About & Support]() |
| Arm Limited, Inc.| [ARM AVH](https://resources.github.com/arm-gihub-actions-beta/)| [About & Support](https://arm-software.github.io/AVH/main/infrastructure/html/avh_gh.html) |

## How to Interact with the Repo

- **Issues**: To file a bug report, or request tools to be added/updated, please [open an issue using the appropriate template](https://github.com/actions/partner-runner-images/issues/new/choose)
- **Discussions**: If you want to share your thoughts about image configuration, installed software, or bring a new idea, please create a new topic in a [discussion](https://github.com/actions/partner-runner-images/discussions) for a corresponding category. Before making a new discussion please make sure no similar topics were created earlier.
- For general questions about using the runner images or writing your Actions workflow, please open requests in the [GitHub Actions Community Forum](https://github.community/c/github-actions/41).

## FAQs

<details>
   <summary><b><i>How does GitHub determine which partners are able to provide images?</b></i></summary>

We are currently reviewing which partnerships are best suited to provide particular experiences in GitHub Actions. If you are interested in providing an image please create an issue in this repo and the GitHub team will reach out to you. 
</details>

<details>
   <summary><b><i>How do I request that a new tool be pre-installed on a particular image?</b></i></summary>
Please create an issue and get an approval from us to add this tool to the image before creating the pull request.
</details>
