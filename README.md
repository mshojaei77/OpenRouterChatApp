# OpenRouter Chat App

This Python script allows users to interact with AI chat models using the OpenRouter API. It provides a simple command-line interface for engaging in conversations with selected AI models.

## Prerequisites

- Python  3.6+
- `aiohttp` library for asynchronous HTTP requests

## Installation

Install the required library by running:

```bash
pip install aiohttp
```

## Usage

Run the script using:

```bash
python openrouter_chat_app.py
```

## Features

- **Model Selection**: Choose from a list of available AI models (you can add more models base on your api here is [Supported Models](https://openrouter.ai/docs#models)).
- **Conversation History**: Maintains the last  30 messages to provide context for AI responses.
- **Asynchronous HTTP Requests**: Utilizes `asyncio` and `aiohttp` for efficient handling of API calls.
- **Rate Limiting**: Implements a semaphore to limit concurrent API requests to  10.

## Configuration

Before running the script, ensure that you have an API key from OpenRouter. You can obtain one from the [OpenRouter Keys page](https://openrouter.ai/keys). Once you have the key, replace the placeholder in the following line with your actual API key:

```python
OPENROUTER_API_KEY = "your_openrouter_api_key_here"
```

Replace `$YOUR_SITE_URL` and `$YOUR_APP_NAME` in the headers with the appropriate values for your application.

## Running the Script

Upon execution, the script will prompt you to select an AI model from the list provided. After selecting a model, you can begin typing messages to interact with the AI. Type `exit` or `quit` to terminate the session.

## Future Updates:

- **Web App Integration**: Plans are underway to develop a web application version of the OpenRouter Chat App using Flask. This will enable users to interact with the AI models via a browser-based interface, providing an alternative to the current command-line approach.

- **Telegram Bot Deployment**: There are plans to integrate the OpenRouter Chat App functionality into a Telegram bot. Users will be able to engage with the AI models directly from their Telegram messenger, offering a convenient way to chat with the AI models on-the-go.

Stay tuned for updates on these features, which aim to expand the reach and usability of the OpenRouter Chat App across different platforms.

## Contributing

Feel free to fork the repository and submit pull requests for improvements or new features.

---

Please note that the actual API URL and header fields (`HTTP-Referer`, `X-Title`) may need to be adjusted according to the specific requirements of [the OpenRouter API](https://openrouter.ai/docs#api-keys)https://openrouter.ai/docs#api-keys.


