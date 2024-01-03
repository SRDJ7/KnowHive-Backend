# KnowHive-Backend
This repository contains the backend code for KnowHive assistant built with Flask, Transformers, and SQLAlchemy.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Introduction

This backend serves as the core of a Conversational AI system that allows users to interact with a fine-tuned GPT-2 model for answering questions related to incident descriptions.

## Features

- User authentication and authorization using Flask-Login
- JWT-based token authentication for secure communication
- MySQL database integration with Flask-SQLAlchemy
- Conversation history tracking for each user
- GPT-2 model fine-tuning and usage for generating answers
- CORS-enabled for cross-origin requests
- Flask-WTF for handling forms
- Flask-Session for managing user sessions

## Setup

1. Clone the repository:
git clone https://github.com/your-username/your-repo.git
cd your-repo

2. Install dependencies:
pip install -r requirements.txt

3. Set up the MySQL database:
Create a MySQL database named conversation_history or update the SQLALCHEMY_DATABASE_URI in app.config accordingly.

4. Run the database migrations:
flask db init
flask db migrate
flask db upgrade

5. Run the Flask app:
python app.py

## Usage
1. Access the application at `http://127.0.0.1:5000/` in your web browser.
2. Use the provided API endpoints for user authentication, asking questions, and retrieving conversation history.
3. Interact with the Conversational AI system using the `/ask` endpoint.

## API Endpoints
* `/login` (POST): User login endpoint.
* `/signup` (POST): User signup endpoint./signup (POST): User signup endpoint.
* `/logout` (GET): User logout endpoint.
* `/conversation-history` (GET): Retrieve user conversation history.
* `/ask` (POST): Ask a question and get a response from the Conversational AI system.
