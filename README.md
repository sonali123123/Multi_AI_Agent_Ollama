# Multi_AI_Agent_Ollama

A collaborative AI system built with Streamlit and Ollama that uses multiple specialized agents to perform complex tasks with validation and refinement.

## Overview
This Multi-Agent AI System demonstrates the power of collaborative AI by using specialized agents for different tasks, with separate validation and refinement steps. The system leverages local LLM models through Ollama to perform three main tasks:

### Medical Text Summarization

### Research Article Writing and Refinement

### Medical Data Sanitization (PHI Removal)

## Features

### Agent Collaboration: Multiple specialized agents work together to complete complex tasks

### Validation Pipeline: Dedicated validation agents ensure quality output

### Refinement Process: Agents that improve and polish initial outputs

### Local LLM Integration: Uses Ollama to run models locally

### User-friendly Interface: Built with Streamlit for easy interaction


## Technology Stack

Python: Core programming language

Streamlit: Web interface framework

Ollama: Local LLM model runner

Loguru: Advanced logging

dotenv: Environment variable management


## Architecture
The system follows a modular architecture with these components:

## Agent Types
Tool Agents: Perform primary tasks (summarize, write articles, sanitize data)
Validator Agents: Evaluate and rate the quality of outputs
Refiner Agent: Improves and polishes initial outputs
Agent Manager: Coordinates and provides access to all agents


## File Structure

app.py: Main application with Streamlit UI and workflow logic

agents/: Directory containing all agent implementations

agent_base.py: Base class for all agents

summarize_tool.py: Summarization agent

write_article_tool.py: Article writing agent

sanitize_data_tool.py: Data sanitization agent

summarize_validator_agent.py: Validates summaries

write_article_validator_agent.py: Validates articles

sanitize_data_validator_agent.py: Validates sanitized data

refiner_agent.py: Refines and improves outputs

validator_agent.py: General validation agent

init.py: Imports and initializes the AgentManager

utils/: Utility functions

logger.py: Logging configuration

logs/: Directory for log files

test.py: Simple test file for Ollama integration


## Installation

Clone the repository:

git clone https://github.com/sonali123123/Multi_AI_Agent_Ollama.git



Navigate to the project directory:

cd Multi_AI_Agent_Ollama

Install the required dependencies:

pip install -r requirements.txt


### Usage

Start the Streamlit application:

streamlit run app.py


Open your browser and navigate to the URL shown in the terminal (typically http://localhost:8501)

## Select a task from the sidebar:

Summarize Medical Text

Write and Refine Research Article

Sanitize Medical Data (PHI)

Follow the on-screen instructions to input your data and run the selected task

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
