# SAP BTP Setup Automator
<!--- Register repository https://api.reuse.software/register, then add REUSE badge:
[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/REPO-NAME)](https://api.reuse.software/info/github.com/SAP-samples/REPO-NAME)
-->

## Description

This repository provides the user with a script to automate the setup of an [SAP BTP account](https://account.hana.ondemand.com/).

This includes:

> - setup of your SAP BTP account
> - entitlement of services
> - deployment of complete applications

In essence it's all about making it easier to get developers quickly onboard on SAP BTP and more easily make use of services on the SAP BTP.

### All on docker

The tooling is running within a docker container and the repository provides all you need to run the tooling in a docker image.
Why docker? We want to ensure that you can focus on getting your work done on the SAP BTP account without having to worry whether you have the right tools in the right release for the right operating system in place.

### The use cases

As a user the only thing you need to focus on is your use case that defines which services or subscriptions you need. The use case is defined within a json structure. You can find a few use cases in the use cases folder of this repository, but you can create your own, if you want to run the script.

## Requirements

To use the tooling you first need to finish the following tasks:

- Get an [SAP BTP trial account](https://cockpit.hanatrial.ondemand.com/trial/#/home/trial) (you can also use a [productive SAP BTP account](https://account.hana.ondemand.com/#/home/welcome))
- [Install a Git client](https://git-scm.com/downloads) - you need it to access the code samples
- [Install a Docker engine](https://docs.docker.com/desktop/)

If you want to have an easier start into the Docker container topic you might want to install **MS Visual Studio Code**, too:

- [Install Visual Studio Code](https://code.visualstudio.com/download) - this will be your development environment
- Install the VS Code plugin for Remote containers ([checkout this great 5 minute video on dev containers](https://www.youtube.com/watch?v=Uvf2FVS1F8k))

## Download and Installation

If the pre-requisites above are all met, you can start your work by creating first your container.

These are the steps:

- clone this Git repository to a local folder on your machine
- open the local folder in a command terminal on your machine (or in VS Code)
- Now you can build the container with the following command. For Mac/Linux

```bash
./run
```

and for MS Windows users:

```bash
.\run.bat
```

This will build a docker image and create a docker container on your machine.

If all went well, you can see the container running in your docker engine.

![command in VS Code to attach it to a running container](docs/pics/quick-guide-step06.png)

![select running container in VS Code](docs/pics/quick-guide-step07.png)

You can run the container directly via the terminal or within Microsoft Visual Studio Code (VSCode).

[Read the instructions for the usage in VSCode](docs/vscode.md).

## Known Issues

Non (so far).

## How to obtain support

[Create an issue](https://github.com/SAP-samples/<repository-name>/issues) in this repository if you find a bug or have questions about the content.

For additional support, [ask a question in SAP Community](https://answers.sap.com/questions/ask.html).

## Contributing

If you wish to contribute code, offer fixes or improvements, please send a pull request. Due to legal reasons, contributors will be asked to accept a DCO when they create the first pull request to this project. This happens in an automated fashion during the submission process. SAP uses [the standard DCO text of the Linux Foundation](https://developercertificate.org/).

## License

Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.