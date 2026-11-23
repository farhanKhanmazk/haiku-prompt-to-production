# haiku-prompt-to-production

Notebooks from my learning journey through the Building with the Claude API course. They cover the Claude API in Python, from basic requests to streaming, stop sequences, and structured output, with a focus on Claude Haiku.

## Contents

- **`001-requests.ipynb`**: basic requests with `claude-sonnet-4-6`, a two-turn conversation, and a simple calculator chat loop.
- **`002-request.ipynb`**: examples with `claude-haiku-5-5`:
  - A `chat()` helper with a system prompt and temperature
  - Streaming responses, both raw events and the text stream
  - Stop sequences, using `</poem>` as the stop marker
  - A short answer capped with `max_tokens`
  - Generating JSON with no extra commentary

## Setup

1. Install the dependencies:
   ```bash
   pip install anthropic python-dotenv
   ```
2. Create a `.env` file in the project folder with your key:
   ```
   ANTHROPIC_API_KEY="your-key-here"
   ```
   Never commit `.env`. The `.gitignore` already excludes it.
3. Open either notebook in Jupyter and run the cells in order.

## Notes

- The notebooks print model output directly, so results will vary between runs.
- `001-requests.ipynb` cell 1 writes the `.env` file. Replace the placeholder with your own key before running it.
