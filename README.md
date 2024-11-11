# DuckDuckGo Chat API Python Client

A Python client for the [DuckDuckGo Chat API](https://duckduckgo.com/aichat) to send messages and receive responses asynchronously. With this .ipynb file, you can use GPT-4o mini, Claude 3 Haiku, Llama 3.1 70B, Mixtral 8x7B for free.

- Inspired from [mumu-lhl/duckduckgo-ai-chat](https://github.com/mumu-lhl/duckduckgo-ai-chat)

## Requirements

- Python 3.7+
- `httpx` library

## Classes

### Model

Available AI models:

- `GPT_4O_MINI`
- `CLAUDE_3_HAIKU`
- `META_LLAMA`
- `MISTRALAI`

## Usage

### Example usage of "gpt-4o-mini"

```python
chat_instance = await init_chat(Model.GPT_4O_MINI)
response = await chat_instance.fetch_full("Merhaba. Nasıl gidiyor?")
print(response)
```

### Example usage of "claude-3-haiku-20240307"

```python
chat_instance = await init_chat(Model.CLAUDE_3_HAIKU)
response = await chat_instance.fetch_full("Merhaba. Nasıl gidiyor?")
print(response)
```

### Example usage of "meta-llama/Meta-Llama-3.1-70B-Instruct-Turbo"

```python
chat_instance = await init_chat(Model.META_LLAMA)
response = await chat_instance.fetch_full("Merhaba. Nasıl gidiyor?")
print(response)
```

### Example usage of "mistralai/Mixtral-8x7B-Instruct-v0.1"

```python
chat_instance = await init_chat(Model.MISTRALAI)
response = await chat_instance.fetch_full("Merhaba. Nasıl gidiyor?")
print(response)
```
