# LangChain Social Post Generator

A small LangChain project that turns short product descriptions into structured social media posts for Cairo-based cafés and shops.

The generator uses Gemini to create:
- A short title
- A caption under 280 characters
- 3-5 hashtags
- Alt-text
- An Arabic translation of the caption

## Tech Stack
- Python
- LangChain
- Google Gemini
- Pydantic
- Google Colab

## Setup

Install the required libraries:

```bash
pip install -U langchain langchain-google-genai pydantic
```

Add a Gemini API key to Google Colab Secrets as:

```
GEMINI_API_KEY
```

Then open `langchain_social_post.ipynb` and run the notebook from top to bottom.

## Test Descriptions

The notebook was tested with:

1. `New iced karak chai with cardamom, served cold in a tall glass.`
2. `Creamy iced karak chai made with black tea, milk, and fragrant cardamom.`
3. `Refreshing iced karak chai served over ice with a sprinkle of ground cardamom.`

## Files

- `langchain_social_post.ipynb` - Colab notebook
- `posts.csv` - 3 generated social media posts
- `screenshots/` - screenshots of the notebook, structured output, and CSV