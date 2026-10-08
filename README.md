# Hotel-Info-Agent
this is a hotel agent which gives answers to customers except for medical, legal, or any law questions.

## Project Overview

Hotel Info Agent is an AI-powered customer service agent designed to answer questions related to hotel information and customer services. The agent can provide helpful responses to customers about hotel-related topics while avoiding responses to medical, legal, or law-related questions. The project demonstrates how an AI agent can be developed, configured, tested, and organized using Python and Azure AI services.

## Features

* Answers hotel and customer-related questions.
* Provides information based on the agent's configured instructions and knowledge.
* Handles natural-language customer questions.
* Avoids answering medical, legal, or law-related questions.
* Organized Python source code for the agent.
* Includes documentation and testing folders.

## Project Structure

```text
Hotel-Info-Agent/
│
├── README.md
├── LICENSE
│
├── src/
│   └── [Python agent code]
│
├── docs/
│   └── setup.md
│
└── tests/
    └── test_agent.py
```

### `/src`

Contains the Python source code used to implement the Hotel Info Agent.

### `/docs`

Contains documentation for setting up, configuring, and using the project.

### `/tests`

Contains test scripts used to verify the agent and its functionality.

### `README.md`

Provides an overview of the project, installation instructions, usage examples, contribution guidelines, and license information.

### `LICENSE`

Contains the project's Apache License 2.0 terms.

## Setup and Installation

### Prerequisites

Before running the project, make sure you have:

* Python 3.10 or later
* Git
* Access to the Azure AI project and resources used by the agent
* The required Python packages listed in `requirements.txt`

### Clone the Repository

Clone this repository to your local computer:

```bash
git clone https://github.com/an1shm7951/Hotel-Info-Agent.git
```

Navigate into the project directory:

```bash
cd Hotel-Info-Agent
```

### Create a Virtual Environment

Create a Python virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

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

If a `requirements.txt` file is not included, install the packages required by the Python agent code and the Azure services used by the project.

### Configuration

Configure the Azure AI project settings and any required credentials before running the agent.

Do not upload API keys, passwords, tokens, or other sensitive credentials to GitHub.

If environment variables are required, store them in a local `.env` file and add `.env` to `.gitignore`.

## Example Usage

After completing the setup and configuration, run the Python agent from the project directory.

For example:

```bash
python src/agent.py
```

The exact Python filename and command may vary depending on the agent implementation.

Example questions that can be asked to the agent include:

```text
What hotel services are available?
What facilities does the hotel provide?
What information can you provide about the hotel?
```

The agent is designed to respond to hotel-related questions and avoid providing medical or legal advice.

## Testing

Test scripts are stored in the `/tests` directory.

If automated tests are available, they can be run using:

```bash
pytest
```

The tests can be used to verify that the agent behaves correctly for supported hotel-related questions and appropriately handles unsupported topics.

## Contribution Guidelines

Contributions are welcome.

To contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make and test your changes.
4. Commit your changes with a clear commit message.
5. Submit a pull request describing the changes.

Please keep contributions focused on improving the functionality, documentation, reliability, or usability of the Hotel Info Agent.

## License

This project is licensed under the Apache License 2.0.

See the `LICENSE` file for the complete license terms.

## Repository

GitHub repository:

https://github.com/an1shm7951/Hotel-Info-Agent
