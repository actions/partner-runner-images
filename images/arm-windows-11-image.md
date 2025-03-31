# Windows 11 by Arm Limited 

The Windows 11 Arm image is created from the [GitHub Actions Runner Images](https://github.com/actions/runner-images) repository.

Some changes have been made to accommodate for the Arm architecture. 
- Some tools do not support Arm and are not available

If you would like something added or would like to propose a substitute for something that does not work on Arm, please open an issue in this repo.

## Installed Software

- Bash
- Go
- Julia
- Kotlin
- LLVM
- Node
- Perl
- PHP 
- Python
- Ruby
- Chocolatey
- Composer
- Helm 
- Miniconda
- NPM
- NuGet
- pip
- Pipx
- RubyGems 
- Vcpkg
- Yarn
- Ant
- Gradle
- Maven
- sbt 
- 7zip
- aria2 
- azcopy 
- Bazel
- Bazelisk 
- Bicep 
- CMake 
- CodeQL 
- Docker 
- Docker Compose v2
- Docker-wincred 
- Git
- ImageMagick 
- InnoSetup 
- jq 
- Kind 
- Kubectl 
- Mercurial 
- gcc 
- gdb 
- GNU Binutils 
- Newman 
- NSIS 
- OpenSSL 
- Packer 
- Pulumi 
- R 
- Stack 
- Swig 
- VSWhere 
- GitBash
- WinAppDriver 
- yamllint 
- Nginx
- Apache
- Alibaba Cloud CLI 
- AWS CLI 
- AWS SAM CLI 
- AWS Session Manager CLI 
- Azure CLI
- Azure DevOps CLI extension
- GitHub CLI 
- Google Chrome 
- Chrome Driver 
- Microsoft Edge Driver 
- Mozilla Firefox 
- Gecko Driver 
- IE Driver 
- Selenium server 
- Java
- Node.js
- Visual Studio
- Powershell

## Omitted software

This section lists tools which are installed on [Windows 2022 X86 image](https://github.com/actions/runner-images/blob/main/images/windows/Windows2022-Readme.md) provided by GitHub but omitted from the current image.

-  Tools that are not available on Windows 11 Arm image
    - Android SDK
    - Cabal
    - Microsoft SQL client tools
    - Subversion (SVN)
    - WiX Toolset
    - zstd
    - PostgreSQL
    - MongoDB
    - Haskell
    - PyPy
    - Msys2
    - pacman
