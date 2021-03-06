# Unofficial Nessus Essential Scanner
<img src="https://img.shields.io/badge/license-GPL-blue" /> <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ciro-mota/nessus-scanner"> <img alt="Docker Image Size (tag)" src="https://img.shields.io/docker/image-size/ciromota/nessus-scanner/latest">

Tenable's Nessus Scanner is a vulnerability scanner that looks for known vulnerabilities, configuration issues and more by inspecting hosts over the network. For more information about Nessus, see the following links:

[Nessus 8.11.x Docs](https://docs.tenable.com/nessus/Content/GettingStarted.htm)

# Requirements

- Docker.
- Debian Slim image Docker.
- License to use Nessus. You can get it [here](https://www.tenable.com/products/nessus/activation-code).

# Build

- Clone this repository.
- Run the command: `docker build -t nessus .`

# Usage

```bash
docker run -td --name nessus -p 8834:8834 -v \
/etc/localtime:/etc/localtime nessus
```