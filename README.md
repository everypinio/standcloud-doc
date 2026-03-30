<div align="center">

[![Documentation](https://img.shields.io/badge/Documentation%20-Overview%20-%20%23007ec6)](https://everypinio.github.io/standcloud-doc/)
[![Discord](https://img.shields.io/discord/1304494076799877172?color=7389D8&label&logo=discord&logoColor=ffffff)](https://discord.gg/98bWadmG8J)
[![Telegram](https://img.shields.io/badge/-Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/everypin)

</div>

---

# StandCloud Documentation

This repository contains the source files for the **StandCloud** project documentation. We use [MkDocs](https://www.mkdocs.org/) with the Material theme to build and serve our docs.

Follow the instructions below to set up your local development environment and preview changes in real-time.

---

## Getting Started

### Prerequisites

Ensure you have **Python 3.x** installed on your system. You can verify this by running:
`python3 --version`

### Setup Instructions

1. **Create a Virtual Environment** It is recommended to use a virtual environment to keep dependencies isolated.
   ```bash
   python3 -m venv .venv
   ```

2. **Activate the Environment** On macOS and Linux:
    ```bash
    source .venv/bin/activate
    ```

    On Windows:
    ```powershell
    .\.venv\Scripts\Activate.ps1
    ```

3. **Install Dependencies** Install the required documentation tools (MkDocs, themes, and plugins):
    ```bash
    pip install -r requirements.txt
    ```

### Local Development

To start the local development server and preview the documentation, run:
```bash
mkdocs serve
```

Once the server is running, open your browser and navigate to:

http://127.0.0.1:8000

The page will automatically reload whenever you save changes to the .md files in the docs/ directory.
