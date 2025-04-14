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

