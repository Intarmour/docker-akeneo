Intarmour Docker Akeneo PIM Community Standard Edition
=====================================

This repository provides Docker configuration files and instructions for setting up Akeneo, a powerful Product Information Management (PIM) system, using Docker containers.


[![CircleCI](https://dl.circleci.com/status-badge/img/circleci/AVKrqpBmkHH4ddomqgsp1c/P7uhDZshJFxAhkyQiEHBFf/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/circleci/AVKrqpBmkHH4ddomqgsp1c/P7uhDZshJFxAhkyQiEHBFf/tree/main)
  <a href="https://github.com/intarmour/docker-magento/graphs/commit-activity" target="_blank"><img src="https://img.shields.io/badge/maintained%3F-yes-brightgreen.svg" alt="Maintained - Yes" /></a>
  <img src="https://img.shields.io/badge/apple%20silicon%20support-yes-brightgreen" alt="Apple Silicon Support" />
  <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>



## Features

- Easy setup and deployment of Akeneo PIM using Docker and Docker Compose.
- Customizable PHP and Apache configurations for fine-tuning performance and functionality.
- MySQL database included with default configuration for seamless integration.
- Access to Akeneo via web browser at `http://localhost:8080` after setup.
- Convenient start and stop commands for managing Docker containers.

## Getting Started

### Prerequisites

- Docker (version >= 19.03.0)
- Docker Compose (version >= 1.25.0)

### Installation

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/Intarmour/docker-akeneo.git
   ```

2. Navigate to the cloned repository:

   ```bash
   cd docker-akeneo
   ```

3. Configure environment variables (if needed) in the `.env` file.

4. Build and start the Docker containers:

   ```bash
   docker-compose up -d --build
   ```

   This command will initialize the Akeneo and MySQL containers defined in the `docker-compose.yml` file.

5. Access Akeneo via your web browser at `http://localhost:8080`.

### Configuration

- MySQL Database Configuration:
  - Host: `db`
  - Port: `3306`
  - Username: `root`
  - Password: `root`
  - Database Name: `akeneo_pim`

### Usage

- Start the containers:

  ```bash
  docker-compose up -d
  ```

- Stop the containers:

  ```bash
  docker-compose down
  ```

## Customization

- Modify PHP and Apache configurations:
  - PHP settings: `docker/php/php.ini`
  - Apache virtual host: `docker/apache/vhost.conf`
- Update `docker-compose.yml` for additional services or configurations.

## Contributing

Contributions are welcome! Please follow the guidelines outlined in [CONTRIBUTING.md](CONTRIBUTING.md) for submitting pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Credits

### Intarmour

<a href="mailto:simone@intarmour.com">💌 Contact me</a>