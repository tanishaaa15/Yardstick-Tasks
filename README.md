# Yardstick-Tasks
## Overview
This notebook implements two core tasks using the Groq API with OpenAI SDK compatibility:

1. Managing Conversation History with Summarization

2. JSON Schema Classification & Information Extraction

The goal is to demonstrate conversational state management, periodic summarization, and structured information extraction—strictly using standard Python and the Groq API client, without frameworks.

## Features
Task 1: Conversation Management & Summarization
- Maintains complete user–assistant conversation history.

- Truncates conversation either by:

- Number of conversation turns (n messages)

- Character length

- Word count

- Performs periodic summarization—summarizes history every k turns and replaces early history with summary for concise memory.

- Configurable: k, n, and truncation mode are easily adjustable.

- Visible printed outputs for each conversation step, showing:

- Current conversation state

- Summaries after each trigger

Task 2: JSON Schema Classification & Extraction
- Defines a strict JSON schema to classify and extract:Name, Email, Phone, Location, Age

- Uses Groq API (OpenAI function/tool calling) to extract structured JSON from chats.

- Validates all output against the schema with error reporting.

- Demonstrates with three diverse example chats.

## Requirements
- Python 3.x recommended.
- Groq API key

## Visible Outputs
Task 1 displays the conversation history after each input, showing where truncation and summarization occur.

Task 2 prints parsed JSON and validation for each chat, highlighting any extraction or format errors.

