# Ubuntu 24.04 by Arm Limited 

The Ubuntu 24.04 LTS Arm image is created from the [GitHub Actions Runner Images](https://github.com/actions/runner-images) repository.

Some changes have been made to accommodate for the Arm architecture. 
- Some tools do not support Arm and are not available
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
- Clang 16, 17, 18
- CMake
- Curl
- Docker
- Docker Compose
- Docker Buildx
- Dotnet (.NET Core)
- g++ (12, 13, 14)
- Gcc (12, 13, 14)
- Git
- Git LFS
- GitHub CLI
- Gradle
- Helm
- Java
- jq
- Lerna
- make
- Maven
- Minikube
- MySQL
- Netlify CLI
- Node.js
- Parcel
- PHP
- Pip
- Pipx
- Pulumi
- PowerShell
- Python
- Ruby
- Rust
- swig
- Swift
- unzip
- Vcpkg
- Yarn
- zip

## Omitted software

This section lists tools which are installed on [Ubuntu 24.04 X64 image](https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2404-Readme.md) provided by GitHub but omitted from the current image.

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
    - NVM (Node Version Manager)
    - OpenShift CLI
    - ORAS CLI
    - PostgreSQL
    - sbt
