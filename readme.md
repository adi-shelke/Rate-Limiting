# Rate Limiting API with Hono and Upstash Redis

This project demonstrates how to implement rate limiting in a serverless API using Hono, a fast, simple, and powerful web framework for Cloudflare Workers, and Upstash Redis, a serverless Redis service.

## Features

- **Rate Limiting**: Protects the `/todos/:id` endpoint from excessive requests by IP address.
- **Serverless**: Built for Cloudflare Workers, leveraging the power and scalability of serverless architecture.
- **Redis-backed**: Utilizes Upstash Redis for storing rate limit counters in a fast, scalable, and serverless data store.

## Getting Started

### Prerequisites

- Node.js installed on your machine.
- A Cloudflare Workers account.
- An Upstash account for Redis.

### Installation

1. Clone the repository to your local machine:

   ```sh
   git clone https://github.com/your-username/rate-limiting.git
   cd rate-limiting

2. Install the dependencies:
    ```sh
    npm install
3. Configure your Redis URL and token by copying the .env.example file to a new file named .env and filling in your Upstash Redis URL and token:
    ```sh
    cp .env.example .env

### Development
* To start the development server, run:
    ```sh
    npm run dev
    
### Usage
* The API has a single endpoint /todos/:id which returns a todo item by its ID. The rate limiting is applied per IP address to prevent excessive requests.

### Contributing
* Contributions are welcome! Please feel free to submit a pull request.
    