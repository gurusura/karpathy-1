# Karpathy
An agentic Machine Learning Engineer

## Setup

### 1. Install and Authenticate Claude Code

For detailed installation and authentication instructions, visit: https://www.claude.com/product/claude-code

### 2. Environment Variables

Copy the `.env.example` file to `.env` in the `karpathy` sub-directory and fill in your API keys:

```bash
cp karpathy/.env.example karpathy/.env
```

Then edit `karpathy/.env` with your actual API key:

```bash
OPENROUTER_API_KEY=your_openrouter_api_key_here
```

The `OPENROUTER_API_KEY` is required for the agent to function properly.

### 3. Install Dependencies

Make sure you have the required dependencies installed. If using `uv`:

```bash
uv sync
```

Or with pip:

```bash
pip install -e .
```

## Quick Start

To setup the sandbox and start the ADK web interface, simply run:

```bash
python start.py
```

This will automatically:
1. Setup the sandbox environment
2. Start the ADK web interface

## Manual Usage

If you want to run the ADK web interface manually without the setup script:

```bash
adk web karpathy
```

**Important:** Always specify the `karpathy` directory when running `adk web`. If you run `adk web` without specifying a directory, it will scan all directories (including `sandbox`) and incorrectly show them as agents.
