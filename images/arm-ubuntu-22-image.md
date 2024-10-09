# Ubuntu 22.04 by Arm Limited 

The Ubuntu 22.04 LTS image with tools is created from the [GitHub Actions Runner Images](https://github.com/actions/runner-images) repository. 

Some changes have been made to accommodate for the Arm architecture. 
- Some tools do not support the Arm and are not available
- Some tools do work on Arm, but have been excluded because they are infrequently used

If you would like something added or would like to propose a substitute for something that does not work on Arm, please open an issue in this repo.

## Installed Software

- 7z
- Ant
- Aria2
- AWS CLI
- Azure CLI
- AzCopy
- Bazel
- Bazelisk
- Bison
- Brotli
- Cargo
- Clang 13, 14, 15
- CMake
- Curl
- Docker
- Docker Compose
- Docker Buildx
- Dotnet (.NET Core)
- g++ (9, 10, 11, 12, 13)
- Gcc (9, 10, 11, 12, 13)
- Git
- Git LFS
- GitHub CLI
- Google Cloud CLI
- Gradle
- Helm
- Java
- jq
- Kotlin
- Lerna
- make
- Maven
- Minikube
- Mono
- Mozilla Firefox
- Netlify CLI
- Node.js
- NuGet
- Packer
- Parcel
- PHP
- Pip
- Pipx
- Pulumi
- PowerShell
- Python
- Ruby
- Rust
- SVN
- swig
- Swift
- Terraform
- unzip
- Vcpkg
- Vercel CLI
- Yarn
- zip

## Not installed software

This section lists tools which are installed on [Ubuntu 22.04 X64 image](https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2204-Readme.md) provided by GitHub but not installed on the current image.

-  Tools that are not supported on Arm architecture
    - Android SDK
    - Edge browser
    - Chrome browser
    - Homebrew (no packages for Arm Linux)
    - R 
    - Microsoft SQL client tools
    - CodeQL

- Infrequently used tools
    - Ansible
    - Alibaba Cloud CLI
    - Azure Bicep
    - Podman and associated container tools
    - Haskell
    - Heroku
    - HHVM (HipHop VM)
    - Julia
    - Leiningen
    - Miniconda
    - MySQL
    - NVM (Node Version Manager)
    - OpenShift CLI
    - ORAS CLI
    - PostgreSQL
    - sbt
