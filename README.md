# Canvas API Token and Course List Retrieval

This project contains a Jupyter Notebook that demonstrates how to interact with the Canvas LMS API to retrieve course-related data using an API token.

## Table of Contents

- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Getting the Canvas API Token](#getting-the-canvas-api-token)
- [Notes](#notes)
- [License](#license)

## Project Overview

The notebook `get-course-list.ipynb` provides an example of how to use the Canvas LMS API to retrieve a list of courses for a given user. You'll need a Canvas API token for authentication. This token must be generated manually by following the steps below.

## Requirements

- Python 3.x
- `python-dotenv` (optional, for managing environment variables)
- Jupyter Notebook (or VSCode Jupyter Extensions)
- Internet access to connect with the Canvas API

### Python Packages
The following Python libraries are required:

- `requests`
- `python-dotenv`
- `pandas` (optional, for organizing and viewing data)

To install them, run the following command:

```bash
pip install requests python-dotenv pandas
```

You can store the Canvas API token in an .env file for convenience. Example:

```bash
# .env file
CANVAS_API_TOKEN=your-canvas-api-token-here
To load the token from this file, ensure you use the python-dotenv package to read the .env file in your notebook.
```

## Getting the Canvas API Token

Follow these steps to get your API token from Canvas:

1. Log in to your Canvas account.
2. Navigate to **Account** in the left-hand sidebar.
3. Click on **Settings**.
4. Scroll down to **Approved Integrations**.
5. Click the button **+ New Access Token**.
6. Give the token a purpose and set an expiration date if needed.
7. Click **Generate Token**.
8. Copy the token and store it in a secure place.

This token will be used for authenticating API requests to Canvas.

## Security Notes

- Be sure to **keep your API token secure**. Do not share it publicly or commit it to version control.
- The API token grants access to your Canvas account, so ensure you understand the permissions granted.