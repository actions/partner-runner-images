
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

This repository contains the information about the VM images provided by GitHub partners which can be used on [GitHub-hosted runners](https://docs.github.com/en/actions/using-github-hosted-runners/using-github-hosted-runners/about-github-hosted-runners). 
The images provided for IBM hardware are for use with GitHub Self-hosted runners however IBM provides a service at no-charge to use the images in IBM Cloud.

Partner images are VM images which are created by third parties which GitHub Hosted Action runner customers can use to improve particular use cases in their workflow by providing particular tools in 'one click' to work with. 

The purpose of this repository is provide a place for users of the images to report bugs and provide feedback on the images. The IBM images are [open source](https://github.com/IBM/action-runner-image-pz) however the other images are not open source, and thus there is no code housed here for building the images themselves. This is a forum for discussions and issues to be raised about the images, as well as a resource for information about the packages and tools on the images. If there is an issue with the underlying hardware, or with Actions, please report issues to GitHub directly using [support](https://support.github.com/request) or [community forums](https://github.com/orgs/community/discussions). You can [report issues related to IBM images](https://github.com/IBM/actionspz/issues).

Please note that since this repository is maintained by partners, it will not provide the same parity of resources that the runner-images repository provides. Each partner will keep the information up to date in this repository to the best of their abilities.

## Available Images

| Partner | Image | YAML Label | Included Software | OS / Architecture | Rollout Progress of Latest Image Release | Support Link | 
|-----------| --------------------|---------------------|--------------------|--------------------|----------------------------|-----------------------|
| Arm Limited, Inc. | Ubuntu 24.04 by Arm Limited | `ubuntu-24.04-arm` and custom in larger runners| [Ubuntu 24.04 Inventory](/images/arm-ubuntu-24-image.md) | Linux, ARM64 | generally available | [About & Support](https://github.com/actions/partner-runner-images/issues/new/choose) |
| Arm Limited, Inc. | Ubuntu 22.04 by Arm Limited | `ubuntu-22.04-arm` and custom in larger runners| [Ubuntu 22.04 Inventory](/images/arm-ubuntu-22-image.md) | Linux, ARM64 | generally available | [About & Support](https://github.com/actions/partner-runner-images/issues/new/choose) |
| Arm Limited, Inc. | Windows 11 by Arm Limited | `windows-11-arm` and custom in larger runners| [Windows 11 Inventory](/images/arm-windows-11-image.md) | Windows, ARM64 | generally available | [About & Support](https://github.com/actions/partner-runner-images/issues/new/choose) |
| IBM | Ubuntu 22.04 | `ubuntu-22.04-ppc64le` | [ubuntu-22.04-ppc64le Binaries Available](https://github.com/IBM/actionspz/blob/main/docs/unsupported-binaries.md) | Linux, ppc64le | generally available | [About actionspz](https://github.com/IBM/actionspz/blob/main/docs/FAQ.md) & [actionspz Support](https://github.com/IBM/actionspz/issues) |
| IBM | Ubuntu 22.04 | `ubuntu-22.04-s390x` | [ubuntu-22.04-s390x Binaries Available](https://github.com/IBM/actionspz/blob/main/docs/unsupported-binaries.md) | Linux, s390x | generally available | [About actionspz](https://github.com/IBM/actionspz/blob/main/docs/FAQ.md) & [actionspz Support](https://github.com/IBM/actionspz/issues) |
| IBM | Ubuntu 24.04 | `ubuntu-24.04-ppc64le` | [ubuntu-24.04-ppc64le Binaries Available](https://github.com/IBM/actionspz/blob/main/docs/unsupported-binaries.md) | Linux, ppc64le | generally available | [About actionspz](https://github.com/IBM/actionspz/blob/main/docs/FAQ.md) & [actionspz Support](https://github.com/IBM/actionspz/issues) |
| IBM | Ubuntu 24.04 | `ubuntu-24.04-s390x` | [ubuntu-24.04-s390x Binaries Available](https://github.com/IBM/actionspz/blob/main/docs/unsupported-binaries.md) | Linux, s390x | generally available | [About actionspz](https://github.com/IBM/actionspz/blob/main/docs/FAQ.md) & [actionspz Support](https://github.com/IBM/actionspz/issues) |

## Current Partner image overview 

### Ubuntu 24.04 by Arm Limited
The image has the most popular tools pre-installed. Check the [image documentation](/images/arm-ubuntu-24-image.md) for more details. **It is a recommended image to use with Linux Arm64 Runners.**

### Ubuntu 22.04 by Arm Limited
The image has the most popular tools pre-installed. Check the [image documentation](/images/arm-ubuntu-22-image.md) for more details. **It is a recommended image to use with Linux Arm64 Runners.**

### Windows 11 by Arm Limited
The image has the most popular tools pre-installed. Check the [image documentation](/images/arm-windows-11-image.md) for more details. **It is a recommended image to use with Windows Arm64 Runners.** 

### Images for IBM Power (ppc64le) and IBM Z (s390x)
The [self-hosted IBM runner image](https://github.com/IBM/action-runner-image-pz) is under the Apache 2.0 License. The image supports multiple environments for both s390x and ppc64le including VM, LXD container, Docker, and Podman. You can [request to use our images in IBM Cloud](https://github.com/IBM/actionspz/issues).

### Blogs
- [Accelerate your CI/CD with Arm-based hosted runners in GitHub Actions](https://github.blog/changelog/2023-10-30-accelerate-your-ci-cd-with-arm-based-hosted-runners-in-github-actions/)
- [GitHub Actions: Simplifying Arm-based Application Development](https://newsroom.arm.com/blog/github-arm-integration)
- [Windows arm64 hosted runners now available in public preview](https://github.blog/changelog/2025-04-14-windows-arm64-hosted-runners-now-available-in-public-preview/)
- [Announcing GitHub Actions avialable for IBM Power, IBM Z and IBM LinuxONE](https://community.ibm.com/community/user/blogs/mick-tarsel/2025/06/23/github-actions-power-z)

### [ARM AVH Image](https://arm-software.github.io/AVH/main/infrastructure/html/avh_gh.html)
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

A GA (General Availability) image has been through a Beta period and is deemed ready for general use. Images are updated on a quarterly cadence. In order to be moved to GA, the image must meet the following criteria:

1. Has been through a Beta period (public or private)
2. Most major software we install on the image has a compatible version for the underlying OS
3. All major bugs reported during the Beta period have been addressed

Any workflows that run on a partner image do not fall under the customer [SLA](https://github.com/customer-terms/github-online-services-sla) as GitHub cannot commit to the partner updating the image within these timeframes. 

## Software and Image Support

### Support Policy

- Updates to each image are owned and managed by the partner providing the image, not GitHub
- GitHub makes no warranties or guarantees for the images or their contents 
- Each partner image will have a different term of support depending on the partner, partner support links can be found below

## How to Interact with the Repo

- **Issues**: To file a bug report, or request tools to be added/updated, please [open an issue using the appropriate template](https://github.com/actions/partner-runner-images/issues/new/choose)
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
