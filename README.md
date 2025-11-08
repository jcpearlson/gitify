# Gitify

TDLR: Use LLM to create commit messages quickly and accurately.  
```
             88           88     ad88               
             ""    ,d     ""    d8"                 
                   88           88                  
 ,adPPYb,d8  88  MM88MMM  88    88     `8b     d8'  
8b       88  88    88     88    88      `8b   d8'   
"8a,   ,d88  88    88,    88    88       `8b,d8'    
 `"YbbdP"Y8  88    "Y888  88    88         Y88'     
 aa,    ,88                                d8'      
  "Y8bbdP"                                d8'       
```

## Project Description

`gitify` is a command-line interface (CLI) tool designed to streamline your Git workflow by leveraging the power of Large Language Models (LLMs). It automates the generation of high-quality Git commit messages and can assist in creating or updating `README.md` files, making your development process more efficient and your project documentation more consistent.

## Features

- **Automated Commit Message Generation:** `gitify` analyzes your staged Git changes and generates descriptive and accurate commit messages using an integrated LLM.
- **Python-based CLI:** A user-friendly command-line interface built with Python.

## Installation

To install `gitify`, you'll need Python 3.8 or higher. It's recommended to install it in a virtual environment.

```bash
# Clone the repository
git clone https://github.com/your-username/gitify.git
cd gitify

# Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate

# Install the package
pip install .
```

Alternatively, if the package is published on PyPI, you can install it directly:

```bash
pip install gitify
```

## Configuration

To use `gitify`, you need to configure your API key and preferred model. This is done using the `config` command.

```bash
gitify config --api_key YOUR_API_KEY --model YOUR_MODEL
```

- `--api_key`: Your API key for the LLM provider (e.g., OpenAI).
- `--model`: The model you want to use for generating commit messages (e.g., `gpt-4`). The default is `gpt-4`.

This will save your configuration to a file named `.gitifyconfig` in your home directory.

**Important:** Keep your API keys secure and do not share them.

## Usage

Once installed, you can use `gitify` from your terminal.

### Generating a Commit Message

To generate a commit message for your staged changes:

```bash
git add .
gitify commit
```

`gitify` will analyze your staged changes and propose a commit message. You will have an option to accept, edit, or regenerate the message.

### Other Commands

For a full list of commands and options:

```bash
gitify --help
```

## Contributing

We welcome contributions!
