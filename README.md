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
+ NPM
### Github Docker Registry

This is [Github Action](https://github.com/jveraduran/container-registry) example about using [Github Docker Registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry)
```
name: Create and publish a Docker image

on:
  release:
    types: [published]

env:
  REGISTRY: ghcr.io
  IMAGE_NAME: ${{ github.repository }}

jobs:
  build-and-push-image:
    runs-on: ubuntu-latest
    permissions:
      contents: read
      packages: write

    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Log in to the Container registry
        uses: docker/login-action@f054a8b539a109f9f41c372932f1ae047eff08c9
        with:
          registry: ${{ env.REGISTRY }}
          username: ${{ github.actor }}
          password: ${{ secrets.PAT_GITHUB_TOKEN }}

      - name: Extract metadata (tags, labels) for Docker
        id: meta
        uses: docker/metadata-action@98669ae865ea3cffbcbaa878cf57c20bbf1c6c38
        with:
          images: ${{ env.REGISTRY }}/${{ env.IMAGE_NAME }}

      - name: Build and push Docker image
        uses: docker/build-push-action@ad44023a93711e3deb337508980b4b5e9bcdc5dc
        with:
          context: .
          push: true
          tags: ${{ steps.meta.outputs.tags }}
          labels: ${{ steps.meta.outputs.labels }}
```
https://docs.github.com/en/actions/security-guides/encrypted-secrets
https://docs.github.com/es/actions/using-workflows/events-that-trigger-workflows#release
https://docs.github.com/es/actions/publishing-packages/publishing-docker-images
+ Infrastructure Modules
+ Ansible Roles
+ Re-usable workflows

## Creating secure code at the beginning

OSS + GHAS (Enterprise)

https://docs.github.com/es/enterprise-cloud@latest/get-started/learning-about-github/about-github-advanced-security

## Metrics as continuos improvement enabler
