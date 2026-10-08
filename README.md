# Hotel Info Agent

## Project Overview

Hotel Info Agent is an AI-powered hotel concierge agent developed using Azure AI Foundry. The agent is designed to interact with users and provide helpful responses to hotel-related questions and customer requests. The project demonstrates how an AI agent can be accessed and used programmatically through Python and the Azure AI Projects SDK. The agent connects to an Azure AI Foundry project, creates a conversation thread, sends a user message, processes the agent's response, and displays the resulting conversation.

## Features

* Connects to an AI agent hosted in Azure AI Foundry.
* Uses Python to communicate with the Azure AI agent.
* Creates conversation threads for user interactions.
* Sends user messages to the Hotel Concierge agent.
* Processes agent runs and retrieves responses.
* Displays the conversation messages in the terminal.
* Uses Azure authentication through `DefaultAzureCredential`.

## Project Structure

```text
Hotel-Info-Agent/
│
├── README.md
├── LICENSE
├── requirements.txt
│
├── src/
│   └── agent.py
│
├── docs/
│   └── setup.md
│
└── tests/
    └── test_agent.py
```

### src

Contains the Python source code used to connect to and interact with the Hotel Info Agent in Azure AI Foundry.

### docs

Contains additional documentation and setup instructions for the project.

### tests

Contains test scripts used to verify the project and its required dependencies.

## Setup and Installation

### Prerequisites

Before running the project, make sure you have:

* Python 3.10 or later
* Git
* An Azure account
* Access to the Azure AI Foundry project containing the Hotel Concierge agent
* Azure CLI for local Azure authentication

### Clone the Repository

Clone the repository using Git:

```bash
git clone https://github.com/an1shm7951/Hotel-Info-Agent.git
```

Navigate to the project directory:

```bash
cd Hotel-Info-Agent
```

### Create a Virtual Environment

Create a Python virtual environment:

```bash
python -m venv .venv
```

On Windows, activate the virtual environment with:

```bash
.venv\Scripts\activate
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

### Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

The project uses the following main packages:

* `azure-ai-projects`
* `azure-identity`
* `pytest`

## Azure Authentication

The project uses `DefaultAzureCredential` from the Azure Identity SDK to authenticate with Azure.

For local development, sign in to Azure using the Azure CLI:

```bash
az login
```

Make sure the signed-in Azure account has access to the Azure AI Foundry project used by the agent.

## Example Usage

Run the agent from the project directory:

```bash
python src/agent.py
```

The Python program connects to the Azure AI Foundry project and retrieves the configured Hotel Concierge agent.

It then creates a conversation thread and sends the following example message:

```text
Hi Hotel Concierge agent
```

The agent processes the request and the resulting conversation messages are displayed in the terminal.

An example output may look similar to:

```text
Created thread, ID: <thread-id>
user: Hi Hotel Concierge agent
assistant: <agent response>
```

The exact response will depend on the configuration and instructions of the Hotel Concierge agent in Azure AI Foundry.

## Testing

Tests are located in the `tests` directory.

Run the tests using:

```bash
pytest
```

The tests verify that the required Python dependencies are available for the project.

## Security

Authentication is handled using Azure's `DefaultAzureCredential`.

Do not commit passwords, API keys, access tokens, or other sensitive credentials to the repository.

Azure credentials should be managed through appropriate Azure authentication methods and environment configuration.

## Contribution Guidelines

Contributions are welcome.

To contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make and test your changes.
4. Commit your changes with a clear commit message.
5. Submit a pull request describing your changes.

Please keep contributions focused on improving the agent, documentation, testing, or project organization.

## License

This project is licensed under the Apache License 2.0.

See the `LICENSE` file for the complete license terms.

## Repository

GitHub repository:

https://github.com/an1shm7951/Hotel-Info-Agent
