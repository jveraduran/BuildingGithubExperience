# Building CI/CD Developers Experience with GitHub

<p align="left" style="text-align:left;">
  <a href="https://www.githubuniverse.com/">
    <img alt="Github Universe" src="img/github-universe-2022.png" width="1040"/>
  </a>
</p>

## About this article 

GitHub with GitHubActions and GHAS offer an incredible experience for developers around the planet. Just with a few considerations and good ideas we can build a wonderful experience for our development teams, and they just literally “work only on their code”

## Code as a company asset

https://dzone.com/articles/source-code-asset-not

## Coexistence Agreements

**Owner Accountability**
+ Teams: Teams + Member Roles, Custome Roles
+ Teams Discussion
+ Repository: Labels, Roles, Topics, Member Privileges
+ Github Actions Workflows - General Topics
+ Organization Secrets

**Development Teams Accountability**

+ Templates
+ Branches + Protection Rules
+ Github Actions - Particular Topics

## Developers diversity with an unique experience

+ Data
+ Infrastructure
+ Front-end
+ Back-End
+ Native Apps

## Complement your experience with your own products

+ Actions Marketplace

### Github NPM Registry
GitHub Packages is a software package hosting service provided by GitHub that allows you to host your software packages such as npm, docker, gem, dotnet, mvn, gradle in privately or publicly and use packages as dependencies in your projects.

You can integrate GitHub Packages with GitHub APIs, GitHub Actions, and webhooks to create an end-to-end DevOps workflow that includes your code, CI, and deployment solutions.

A package is a file or directory that is described by a package.json file. A package must contain a package.json file in order to be published to the npm registry. For more information on creating a package.json file, see "Creating a package.json file".

Packages can be unscoped or scoped to a user or organization, and scoped packages can be private or public

**¿Why use a Private Registry?**

+ **Central hub for all your required package versions:** Private and public together, possibly from multiple upstream sources.
  
+ **Identification and visualization of dependencies:** With all required packages in one place it enables identification of potential issues. Additionally the proxy caches your packages, removing the worry that an essential package version will be unpublished in the future.
  
+ **Single package source:** With all developers using the same registry that contains the same versions, you can ensure all users build and test consistently. Removing the potential issue of unknowingly using different versions of a dependency.

This is a [Github Repository](https://github.com/jveraduran/github-npm-registry-be) with a Back-End Example about using [Github NPM Registry](https://docs.github.com/es/packages/working-with-a-github-packages-registry/working-with-the-npm-registry). ¿Do you have any doubt?, please feel you free to open and issue.

<br>

<p align="left" style="text-align:left;">
  <a href="https://github.com/features/packages">
    <img alt="Github Packages" src="img/packages-benefits.png" width="1040"/>
  </a>
</p>

<br>

### Github Container Registry

GitHub Packages is a software package hosting service provided by GitHub that allows you to host your software packages such as npm, docker, gem, dotnet, mvn, gradle in privately or publicly and use packages as dependencies in your projects.

You can integrate GitHub Packages with GitHub APIs, GitHub Actions, and webhooks to create an end-to-end DevOps workflow that includes your code, CI, and deployment solutions.

Container image registries can offer significant advantages for developers but with one caveat attached: not all registries are created equally.

Public registry services are basic, simple to use and can work well for individuals and smaller teams. But once teams begin to scale up, they run into numerous issues with public registries. A private container registry with scanning capabilities and role-based access control offers more security, governance and efficient management

**¿Why Use a Container Image Registry?**

The registry remains a source of truth for the images you want to run. The first advantage is you have the same piece of code running everywhere. The second advantage is that piece of code is guarded in a repository controlled by IT so you can easily revert to a clean environment. The result is the end of “config drift” in production

**¿What is Github Container Registry?**

The [Container registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry) stores container images within your organization or personal account, and allows you to associate an image with a repository. You can choose whether to inherit permissions from a repository, or set granular permissions independently of a repository. You can also access public container images anonymously.

<br>

<p align="left" style="text-align:left;">
  <a href="https://github.com/features/packages">
    <img alt="Github Packages" src="img/packages-benefits.png" width="1040"/>
  </a>
</p>

<br>

This is a [Github Repository](https://github.com/jveraduran/container-registry) example about using [Github Container Registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry). ¿Do you have any doubt?, please feel you free to open and issue.

+ Infrastructure Modules
+ Ansible Roles
+ Re-usable workflows

## Creating secure code at the beginning

OSS + GHAS (Enterprise)

https://docs.github.com/es/enterprise-cloud@latest/get-started/learning-about-github/about-github-advanced-security

## Metrics as continuos improvement enabler
