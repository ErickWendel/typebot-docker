# Typebot Docker Deployment

A Docker configuration for deploying Typebot with SSL support across multiple ports.

## Overview

This project provides a containerized setup for Typebot, allowing you to quickly deploy the platform with proper SSL configuration. The setup exports Typebot services to different ports while maintaining secure connections.

## Features

- 🔒 SSL support out of the box
- 🐳 Complete Docker-based deployment
- 🚀 Multi-port configuration for different Typebot services
- 🔄 Easy to setup and maintain

## Prerequisites

- Docker and Docker Compose installed
- A domain name pointed to your server
- Basic understanding of Docker concepts

## Quick Start

1. Clone this repository:
   ```
   git clone https://github.com/erickwendel/typebot-docker.git
   cd typebot-docker
   ```

2. Configure environment variables in the `.env` file

3. Start the containers:
   ```
   docker-compose up
   ```

4. Access your Typebot instance at your configured domain

## Important Notes

⚠️ **Storage Configuration**: It is highly recommended to use MinIO or AWS S3 for asset storage in production environments. 

## Environment Variables

Key environment variables to configure:

- `NEXTAUTH_URL`: The URL of your Typebot builder
- `NEXT_PUBLIC_VIEWER_URL`: The URL of your Typebot viewer
- `DATABASE_URL`: PostgreSQL connection string
- `ENCRYPTION_SECRET`: Secret for encrypting sensitive data

See the `.env` file for a complete list of configuration options.

## Credit

This project was originally created as part of a YouTube tutorial by [Erick Wendel](https://www.youtube.com/@ErickWendelAcademy).

## Hosting

This project has been successfully deployed on [Hostinger](https://ewbr.cc/hostinger-maio).

## License

MIT

## Support

If you find this project helpful, please give it a ⭐ on GitHub and subscribe to [Erick Wendel's YouTube channel](https://youtube.com/c/ErickWendelTreinamentos) for more tutorials. 