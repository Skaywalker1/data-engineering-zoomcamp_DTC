# Introduction

* [![](https://markdown-videos-api.jorgenkh.no/youtube/AtRhA-NfS24)](https://www.youtube.com/watch?v=X8cEEwi8DTM)
* [Slides](https://docs.google.com/presentation/d/1974w3_zdaK7tDQJCcxHginiAuN0hRRYqXiHbDWcuVVg/edit?usp=drivesdk)
* Overview of [Architecture](https://github.com/DataTalksClub/data-engineering-zoomcamp#overview), [Technologies](https://github.com/DataTalksClub/data-engineering-zoomcamp#technologies) & [Pre-Requisites](https://github.com/DataTalksClub/data-engineering-zoomcamp#prerequisites)


We suggest watching videos in the same order as in this document.

The last video (setting up the environment) is optional, but you can check it earlier
if you have troubles setting up the environment and following along with the videos.


# Docker + Postgres

[Code](2_docker_sql)

## :movie_camera: Introduction to Docker

[![](https://markdown-videos-api.jorgenkh.no/youtube/EYNwNlOrpr0)](https://youtu.be/EYNwNlOrpr0&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=4)

* Why do we need Docker
* Creating a simple "data pipeline" in Docker


## :movie_camera: Ingesting NY Taxi Data to Postgres

[![](https://markdown-videos-api.jorgenkh.no/youtube/2JM-ziJt0WI)](https://youtu.be/2JM-ziJt0WI&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=5)

* Running Postgres locally with Docker
* Using `pgcli` for connecting to the database
* Exploring the NY Taxi dataset
* Ingesting the data into the database

> [!TIP]
>if you have problems with `pgcli`, check this video for an alternative way to connect to your database in jupyter notebook and pandas.
>
> [![](https://markdown-videos-api.jorgenkh.no/youtube/3IkfkTwqHx4)](https://youtu.be/3IkfkTwqHx4&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=6)


## :movie_camera: Connecting pgAdmin and Postgres

[![](https://markdown-videos-api.jorgenkh.no/youtube/hCAIVe9N0ow)](https://youtu.be/hCAIVe9N0ow&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=7)

* The pgAdmin tool
* Docker networks


> [!IMPORTANT]
>The UI for PgAdmin 4 has changed, please follow the below steps for creating a server:
>
>* After login to PgAdmin, right click Servers in the left sidebar.
>* Click on Register.
>* Click on Server.
>* The remaining steps to create a server are the same as in the videos.


## :movie_camera: Putting the ingestion script into Docker

[![](https://markdown-videos-api.jorgenkh.no/youtube/B1WwATwf-vY)](https://youtu.be/B1WwATwf-vY&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=8)

* Converting the Jupyter notebook to a Python script
* Parameterizing the script with argparse
* Dockerizing the ingestion script

## :movie_camera: Running Postgres and pgAdmin with Docker-Compose

[![](https://markdown-videos-api.jorgenkh.no/youtube/hKI6PkPhpa0)](https://youtu.be/hKI6PkPhpa0&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=9)

* Why do we need Docker-compose
* Docker-compose YAML file
* Running multiple containers with `docker-compose up`

## :movie_camera: SQL refresher

[![](https://markdown-videos-api.jorgenkh.no/youtube/QEcps_iskgg)](https://youtu.be/QEcps_iskgg&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=10)

* Adding the Zones table
* Inner joins
* Basic data quality checks
* Left, Right and Outer joins
* Group by

## :movie_camera: Optional: Docker Networking and Port Mapping

> [!TIP]
> Optional: If you have some problems with docker networking, check **Port Mapping and Networks in Docker video**.

[![](https://markdown-videos-api.jorgenkh.no/youtube/tOr4hTsHOzU)](https://youtu.be/tOr4hTsHOzU&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=5)

* Docker networks
* Port forwarding to the host environment
* Communicating between containers in the network
* `.dockerignore` file

## :movie_camera: Optional: Walk-Through on WSL

> [!TIP]
> Optional: If you are willing to do the steps from "Ingesting NY Taxi Data to Postgres" till "Running Postgres and pgAdmin with Docker-Compose" with Windows Subsystem Linux please check **Docker Module Walk-Through on WSL**.

[![](https://markdown-videos-api.jorgenkh.no/youtube/Mv4zFm2AwzQ)](https://youtu.be/Mv4zFm2AwzQ&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=33)


# GCP

## :movie_camera: Introduction to GCP (Google Cloud Platform)

[![](https://markdown-videos-api.jorgenkh.no/youtube/18jIzE41fJ4)](https://youtu.be/18jIzE41fJ4&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=3)

# Terraform

[Code](1_terraform_gcp)

## :movie_camera: Introduction Terraform: Concepts and Overview, a primer

[![](https://markdown-videos-api.jorgenkh.no/youtube/s2bOYDCKl_M)](https://youtu.be/s2bOYDCKl_M&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=11)

* [Companion Notes](1_terraform_gcp)

## :movie_camera: Terraform Basics: Simple one file Terraform Deployment

[![](https://markdown-videos-api.jorgenkh.no/youtube/Y2ux7gq3Z0o)](https://youtu.be/Y2ux7gq3Z0o&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=12)

* [Companion Notes](1_terraform_gcp)

## :movie_camera: Deployment with a Variables File

[![](https://markdown-videos-api.jorgenkh.no/youtube/PBi0hHjLftk)](https://youtu.be/PBi0hHjLftk&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=13)

* [Companion Notes](1_terraform_gcp)

## Configuring terraform and GCP SDK on Windows

* [Instructions](1_terraform_gcp/windows.md)


# Environment setup

For the course you'll need:

* Python 3 (e.g. installed with Anaconda)
* Google Cloud SDK
* Docker with docker-compose
* Terraform
* Git account

> [!NOTE]
>If you have problems setting up the environment, you can check these videos.
>
>If you already have a working coding environment on local machine, these are optional. And only need to select one method. But if you have time to learn it now, these would be helpful if the local environment suddenly do not work one day.

## :movie_camera: GCP Cloud VM

### Setting up the environment on cloud VM
[![](https://markdown-videos-api.jorgenkh.no/youtube/ae-CV2KfoN0)](https://youtu.be/ae-CV2KfoN0&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=14)

* Generating SSH keys
* Creating a virtual machine on GCP
* Connecting to the VM with SSH
* Installing Anaconda
* Installing Docker
* Creating SSH `config` file
* Accessing the remote machine with VS Code and SSH remote
* Installing docker-compose
* Installing pgcli
* Port-forwarding with VS code: connecting to pgAdmin and Jupyter from the local computer
* Installing Terraform
* Using `sftp` for putting the credentials to the remote machine
* Shutting down and removing the instance

## :movie_camera: GitHub Codespaces

### Preparing the environment with GitHub Codespaces

[![](https://markdown-videos-api.jorgenkh.no/youtube/XOSUt8Ih3zA)](https://youtu.be/XOSUt8Ih3zA&list=PL3MmuxUbc_hJed7dXYoJw8DoCuVHhGEQb&index=15)

