# Getting stated with Azure Cloud Adoption Framework landing zones on Visual Studio Codespaces

## Introduction

Visual Studio Codespaces is a browser-based editor with support for Git repos, extensions, and a built-in command line interface so you can edit, run, and debug your applications from any device. For more details on Visual Studio Codespace, you can visit the product page [here](https://visualstudio.microsoft.com/services/visual-studio-codespaces/)

## Prerequisites

In order to start deploying your with CAF landing zones on VS Codespaces, you need:

* an Azure subscription (Trial, MSDN, etc.)

## Create your account

Let's authenticate first:
[https://aka.ms/vso-login](https://aka.ms/vso-login)
![Signin](../../_pictures/getting_started/vs_codespaces_getting_started.png)

## Create the repository in Visual Studio Code

Create the landing zones Codespaces clicking here: [![VScodespaces](https://img.shields.io/endpoint?url=https%3A%2F%2Faka.ms%2Fvso-badge)](https://online.visualstudio.com/environments/new?name=caf%20landing%20zones&repo=azure/caf-terraform-landingzones)

![Create](../../_pictures/getting_started/vs_codespaces_create.png)

The create process will look something like that:

![Create](../../_pictures/getting_started/vs_codespaces_create2.png)

Once ready, you should have your Visual Studio Interface as follow:
![Create](../../_pictures/getting_started/vs_codespaces_create3.png)

Open a Terminal using ```CTRL``` + ```J``` or ```Command``` + ```J```

![Create](../../_pictures/getting_started/vs_codespaces_create4.png)

You are ready to use landing zones by launching the rover as below:

```bash
rover
```

![Create](../../_pictures/getting_started/vs_codespaces_rover.png)

## Deploying your first landing zone

You must be authenticated first:
For that we will rely on Azure authentication as completed by Azure Cli, via browser method:

```bash
rover login
```

We recommend that you verify the output of the login and make sure the subscription selected by default is the one you want to work on. If not, you can use the following switch:

```bash
az account set --subscription <subscription_GUID>
```