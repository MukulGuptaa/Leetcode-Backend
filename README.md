# LeetCode Backend Services

A microservices-based backend architecture for LeetCode-like coding platform.

<img width="597" alt="LeetcodeArchiecture" src="https://github.com/user-attachments/assets/e4c78363-2d9a-40a3-83c8-ea82202c90aa" />

## Overview

This project implements a scalable backend architecture for a LeetCode-like coding platform using microservices. The system is designed to handle code submissions, real-time evaluation, problem management, and socket-based communication.

## Tech Stack

### Core Technologies
- **JavaScript/TypeScript**: Primary programming language
- **Node.js**: Runtime environment
- **Express/Fastify**: Web frameworks for building APIs
- **Socket.IO**: Real-time bidirectional communication
- **Redis**: 
  - Queue management for job processing
  - Caching layer for improved performance
- **Dockerode**: Docker API client for container management

## Services

### 1. LeetCode Submission Service
- Handles code submission requests
- Manages submission queue
- Integrates with evaluation service

### 2. LeetCode Socket Service
- Manages real-time communication
- Handles WebSocket connections
- Broadcasts evaluation results

### 3. LeetCode Problem Service
- Manages problem database
- Handles problem metadata
- Provides problem content and test cases

### 4. LeetCode Evaluator Service
- Executes submitted code
- Runs test cases
- Provides evaluation results

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Redis Server
- Docker
- TypeScript

### Installation

1. Clone the repository:
```bash
git clone [repository-url]
```

2. Install dependencies for each service:
```bash
cd [service-directory]
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```

4. Start Redis server:
```bash
redis-server
```

5. Start the services:
```bash
npm run start
```

## Architecture

The system follows a microservices architecture with the following components:

- **API Gateway**: Routes requests to appropriate services
- **Message Queue**: Handles asynchronous communication
- **Cache Layer**: Improves response times
- **Container Management**: Isolates code execution
- **Real-time Updates**: Socket-based communication

## Development

### Running Tests
```bash
npm run test
```

### Building for Production
```bash
npm run build
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
