# Boilerplates

Welcome to the Docker Compose Boilerplates repository!
It contains several collections, including a collection of Docker Compose configurations helps you quickly set up and deploy various services in a containerized environment. Whether you're a developer, system administrator, or just curious about containerization, these boilerplates make it easy to spin up different services with minimal effort.

> **Notes:**
>
> - These boilerplates are intended for development and testing purposes only. They are not meant to be used in production environments.
>
> - These boilerplates are not meant to be used as-is. You should tweak the configuration files to suit your needs.
>
> - I will be adding more boilerplates in the future, so stay tuned!
>

## Table of Contents

- [Getting Started][1]
  - [Prerequisites][2]
  - [Setup][3]
- [License][4]

## Getting Started

### Prerequisites

- [Docker][5]

    ``` bash
    # Install Docker on Debian-based distros
    sudo apt update
    sudo apt install docker.io
    sudo systemctl start docker
    sudo systemctl enable docker
    # Install Docker on Fedora and CentOS-based distros
    sudo yum install docker
    sudo systemctl start docker
    sudo systemctl enable docker
    # Install Docker on Arch-based distros
    sudo pacman -S docker
    sudo systemctl start docker
    sudo systemctl enable docker
    # Install Docker on macOS
    brew cask install docker
    # Install Docker on Windows
    winget install -e --id Docker.DockerDesktop
    ```

- [Docker Compose][6]

    ``` bash
    # Install Docker Compose on Linux systems
    sudo apt update
    sudo apt install docker-compose
    # Install Docker Compose on macOS
    brew install docker-compose
    ```

    > **Note:** If you're using Windows, Docker Compose is already included in Docker Desktop.

- [Git][7]

    ``` bash
    # Install Git on Debian-based distros
    sudo apt update
    sudo apt install git
    # Install Git on Fedora and CentOS-based distros
    sudo yum install git
    # Install Git on Arch-based distros
    sudo pacman -S git
    # Install Git on macOS
    brew install git
    # Install Git on Windows
    winget install git
    ```

### Setup

Clone this repository:

```bash
git clone https://github.com/younest9/boilerplates.git
```

#### PiHole + Unbound

```bash
cd boilerplates/docker-compose/pihole+unbound
docker-compose up -d
```

> **Note:** You can tweak the configuration by editing the `.env` file, and uncommenting some parameters in the `docker-compose.yml` file.

## License

This project is licensed under the MIT License - see the [LICENSE][8] file for details.

[1]:#getting-started
[2]:#prerequisites
[3]:#setup
[4]:#license
[5]:https://docs.docker.com/install/
[6]:https://docs.docker.com/compose/install/
[7]:https://git-scm.com/downloads
[8]:./LICENCE
