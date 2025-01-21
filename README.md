# Extractive Summarization

# 1. Extractive Summarization with BART

Extractive summarization using a pre-trained BART model from Hugging Face's `transformers` library. The input text is cleaned, chunked to respect model token limits, summarized, and saved as an output file.

---

## Features

1. **Preprocessing**: Cleans the input text by removing special characters and normalizing spaces.
2. **Tokenization-aware Chunking**: Splits text into manageable chunks to adhere to the model's token limit (1024 tokens).
3. **Summarization**: Generates summaries for each chunk using the `facebook/bart-large-cnn` model.
4. **Error Handling**: Handles cases of empty input or model exceptions gracefully.
5. **Output**: Saves the final summarized text to a file for easy use.

---

# 2. Extractive Summarization using Sumy


Extractive summarization using the **Sumy** library, which provides  implementations of algorithms like LexRank and Latent Semantic Analysis (LSA). The input text is summarized into a specified number of sentences and saved as an output file.

---

## Features

1. **Multiple Summarization Methods**:
   - **LexRank**: A graph-based ranking model for text summarization.
   - **LSA**: A statistical method for finding patterns in the relationships between terms.

2. **Configurable Parameters**:
   - Choose the summarization method (`lexrank` or `lsa`).
   - Specify the number of sentences in the summary.

3. **Error Handling**:
   - Handles missing files, invalid methods, and other runtime issues gracefully.

4. **Output**:
   - Summarized text is printed to the console and saved to an output file.

---



