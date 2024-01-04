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

1. __Clone the repository:__
`git clone https://github.com/SRDJ7/KnowHive-Backend`

2. __Install dependencies:__
`pip install -r requirements.txt`

3. __Set up the MySQL database:__
Create a MySQL database named `conversation_history`

4. __Run the Flask app:__
`python app.py`

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

## Azure Deployment Screenshots
<p align="center">
<img width="960" alt="Overview of KnowHive Resource Group in Azure" src="https://github.com/SRDJ7/KnowHive-Backend/assets/67571677/73db9f0a-4e1f-4d94-9419-3cc38f9f40ba">
Overview of KnowHive Resource Group in Azure
</p>

<p align="center">
<img width="960" alt="Overview of deployed KnowHive VM in Azure" src="https://github.com/SRDJ7/KnowHive-Backend/assets/67571677/95f5e7a0-7229-4b68-b366-433eef5b7158">
Overview of deployed KnowHive VM in Azure
</p>

<p align="center">
<img width="960" alt="user table" src="https://github.com/SRDJ7/KnowHive-Backend/assets/67571677/ab655aae-fc9c-4012-8031-1077263c7b2c">
Screenshot of user table in the Azure MySQL DB
</p>

<p align="center">
<img width="960" alt="conversation_history table" src="https://github.com/SRDJ7/KnowHive-Backend/assets/67571677/d7729b9e-50a9-4da3-8302-e24049fb0afa">
Screenshot of conversation_history table in the Azure MySQL DB
</p>
