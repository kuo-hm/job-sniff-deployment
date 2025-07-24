# job-sniff-deployment

This repository manages the deployment and orchestration of the job-sniff microservices architecture.

It contains the master Docker Compose configuration to run all services together, including:

- RabbitMQ message broker  
- PostgreSQL database  
- API Gateway  
- User Service  
- Job Scrapers  

## Usage

1. Copy `.env.sample` to `.env` and update environment variables as needed.  
2. Run `docker-compose up --build` to start the full stack.

## Notes

- This repo references local builds of `job-sniff-core` and `job-sniff-scrapers`. Adjust build paths as necessary.  
- For production, consider secrets management beyond `.env` files.

