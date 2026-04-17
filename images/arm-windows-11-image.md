# Windows 11 by Arm Limited 

The Windows 11 Arm image is created from the [GitHub Actions Runner Images](https://github.com/actions/runner-images) repository.

Some changes have been made to accommodate for the Arm architecture. 
- Some tools do not support Arm and are not available

If you would like something added or would like to propose a substitute for something that does not work on Arm, please open an issue in this repo.

# Windows 11 Enterprise
- OS Version: 10.0.26200 Build 7462
- Image Version: 20260105.41.1
- SKU: win11-25h2-ent 

## Installed Software

### Language and Runtime
- Bash 5.2.37(1)-release
- Go 1.24.11
- Julia 1.12.0
- Kotlin 2.3.0
- LLVM 20.1.6
- Node 24.12.0
- Perl 5.32.1
- PHP 8.4.15
- Python 3.13.11
- Ruby 3.4.7

### Package Management
- Chocolatey 2.6.0
- Composer 2.9.2
- Helm 4.0.3
- NPM 11.6.2
- NuGet 7.0.1.1
- pip 25.3 (python 3.13)
- Pipx 1.8.0
- RubyGems 3.6.9
- Vcpkg (build from commit 544a4c5c29)
- Yarn 1.22.22

#### Environment variables
| Name                    | Value    |
| ----------------------- | -------- |
| VCPKG_INSTALLATION_ROOT | C:\vcpkg |

### Project Management
- Ant 1.10.15
- Gradle 9.1
- Maven 3.9.11
- sbt 1.11.7

### Tools
- 7zip 25.01
- aria2 1.37.0
- azcopy 10.31.1
- Bazel 8.5.0
- Bazelisk 1.26.0
- Bicep 0.39.26
- CMake 4.2.1
- CodeQL Action Bundle 2.23.8
- Git 2.52.0.windows.1
- Git LFS 3.7.1
- ImageMagick 7.1.2-10
- InnoSetup 6.6.1
- jq 1.8.1
- Kind 0.30.0
- Kubectl 1.34.3
- Mercurial 6.3.1
- gcc 14.2.0
- gdb 16.2
- GNU Binutils 2.44
- Newman 6.2.1
- NSIS 3.10
- OpenSSL 3.6.0
- Packer 1.14.2
- Pulumi 3.211.0
- R 4.5.2
- Stack 3.7.1
- Swig 4.3.1
- VSWhere 3.1.7
- WinAppDriver 1.2.2009.02003
- yamllint 1.37.1
- Ninja 1.13.2

### CLI Tools
- Alibaba Cloud CLI 3.2.2
- AWS CLI 2.32.17
- AWS SAM CLI 1.150.1
- AWS Session Manager CLI 1.2.764.0
- Azure CLI 2.81.0
- Azure DevOps CLI extension 1.0.2
- GitHub CLI 2.83.2

### Rust Tools
- Cargo 1.92.0
- Rust 1.92.0
- Rustdoc 1.92.0
- Rustup 1.28.2

#### Packages
- bindgen 0.72.1
- cargo-audit 0.22.0
- cargo-outdated 0.17.0
- cbindgen 0.29.2
- Clippy 0.1.92
- Rustfmt 1.8.0

### Browsers and Drivers
- Google Chrome 143.0.7499.147
- Chrome Driver 143.0.7499.146
- Microsoft Edge 143.0.3650.80
- Microsoft Edge Driver 143.0.3650.80
- Mozilla Firefox 146.0
- Gecko Driver 0.36.0
- IE Driver 4.14.0.0
- Selenium server 4.39.0

#### Environment variables
| Name              | Value                              |
| ----------------- | ---------------------------------- |
| CHROMEWEBDRIVER   | C:\SeleniumWebDrivers\ChromeDriver |
| EDGEWEBDRIVER     | C:\SeleniumWebDrivers\EdgeDriver   |
| GECKOWEBDRIVER    | C:\SeleniumWebDrivers\GeckoDriver  |
| SELENIUM_JAR_PATH | C:\selenium\selenium-server.jar    |

### Java
| Version              | Environment Variable |
| -------------------- | -------------------- |
| 21.0.9+10.0 (default) | JAVA_HOME_21_AARCH64 |
| 23.0.2+7             | JAVA_HOME_23_AARCH64 |

### Cached Tools

#### Go
- 1.22.12
- 1.23.12
- 1.24.11
- 1.25.5

#### Node.js
- 20.19.6
- 22.21.1
- 24.12.0

#### Python
- 3.12.10
- 3.13.11
- 3.14.2

#### Ruby
- 3.4.7

### Database tools
- Azure CosmosDb Emulator 2.14.25.0
- DacFx 170.2.70.1
- MySQL 8.0.44.0
- SQL OLEDB Driver 18.7.5.0

### Web Servers
| Name   | Version | ConfigFile                            | ServiceName | ServiceStatus | ListenPort |
| ------ | ------- | ------------------------------------- | ----------- | ------------- | ---------- |
| Apache | 2.4.55  | C:\tools\Apache24\conf\httpd.conf     | Apache      | Stopped       | 80         |
| Nginx  | 1.29.4  | C:\tools\nginx-1.29.4\conf\nginx.conf | nginx       | Stopped       | 80         |        |

### Visual Studio Enterprise 2022
| Name                          | Version        | Path                                                     |
| ----------------------------- | -------------- | -------------------------------------------------------- |
| Visual Studio Enterprise 2022 | 17.14.36811.4 | C:\Program Files\Microsoft Visual Studio\2022\Enterprise |

#### Installed Windows SDKs
- 10.0.19041.0
- 10.0.22621.0
- 10.0.26100.0

### .NET Core Tools
- .NET Core SDK: 6.0.136, 6.0.203, 6.0.321, 6.0.428, 8.0.122, 8.0.206, 8.0.319, 8.0.416, 9.0.112, 9.0.205, 9.0.308, 10.0.101
- .NET Framework: 4.7.2, 4.8, 4.8.1
- Microsoft.AspNetCore.App: 6.0.5, 6.0.26, 6.0.36, 8.0.6, 8.0.22, 9.0.6, 9.0.11, 10.0.1
- Microsoft.NETCore.App: 6.0.5, 6.0.26, 6.0.36, 8.0.6, 8.0.22, 9.0.6, 9.0.11, 10.0.1
- Microsoft.WindowsDesktop.App: 6.0.5, 6.0.26, 6.0.36, 8.0.6, 8.0.22, 9.0.6, 9.0.11, 10.0.1
- nbgv 3.9.50+6feeb89450

### PowerShell Tools
- PowerShell 7.4.13

#### Powershell Modules
- Az: 12.5.0
- AWSPowershell: 5.0.118
- DockerMsftProvider: 1.0.0.8
- MarkdownPS: 1.10
- Microsoft.Graph: 2.33.0
- Pester: 3.4.0, 5.7.1
- PowerShellGet: 1.0.0.1, 2.2.5
- PSScriptAnalyzer: 1.24.0
- PSWindowsUpdate: 2.2.1.5
- SqlServer: 22.4.5.1
- VSSetup: 2.2.16


## Omitted software

This section lists tools which are installed on [Windows 2022 X86 image](https://github.com/actions/runner-images/blob/main/images/windows/Windows2022-Readme.md) provided by GitHub but omitted from the current image.

-  Tools that are not available on Windows 11 Arm image
    - Android
    - Cabal
    - Docker
    - Docker Compose
    - Docker-wincred
    - Cached Docker images
    - ghc
    - Microsoft SQL client tools
    - Miniconda
    - Service Fabric SDK
    - Subversion (SVN)
    - WiX Toolset
    - zstd
    - PostgreSQL
    - MongoDB
    - Haskell
    - PyPy
    - Msys2
    - pacman
    - SQLPS
