# Karpathy
An agentic Machine Learning Engineer that trains state-of-the-art ML models using Claude Code SDK and Google ADK.

## Prerequisites

- Python 3.13 or higher
- [uv](https://github.com/astral-sh/uv) package manager
- Claude Code installed and authenticated (see [installation guide](https://www.claude.com/product/claude-code))

## Setup

### 1. Install Dependencies

Install dependencies using `uv`:

```bash
uv sync
```

### 2. Environment Variables

Create a `.env` file in the `karpathy` directory with your API keys:

```bash
OPENROUTER_API_KEY=your_openrouter_api_key_here
AGENT_MODEL=your_model_name_here  # Optional: defaults to model configured in ADK
```

The `OPENROUTER_API_KEY` is required for the agent to function properly.

## Quick Start

Run the startup script to set up the sandbox and start the ADK web interface:

```bash
python start.py
```

This automatically:
1. Creates a `sandbox` directory with scientific skills from Claude Scientific Skills
2. Sets up a Python virtual environment with ML packages (PyTorch, transformers, scikit-learn, etc.)
3. Copies your `.env` file to the sandbox
4. Starts the ADK web interface

## Manual Usage

To set up the sandbox without starting the web interface:

```bash
python -m karpathy.utils
```

To run the ADK web interface manually:

```bash
adk web
```

## Enhanced ML Capabilities

If you want substantially more powerful ML capabilities through a multi-agentic system, sign up for [www.k-dense.ai](https://www.k-dense.ai). Currently in closed beta, launching publicly in December 2025.

## Upcoming Features

- **Modal sandbox integration** - Choose any type of compute you want
- **K-Dense Web features** - We might make some features from K-Dense Web available here based on interest

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=K-Dense-AI/karpathy&type=date&legend=top-left)](https://www.star-history.com/#K-Dense-AI/karpathy&type=date&legend=top-left)