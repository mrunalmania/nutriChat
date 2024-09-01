# 🍏 nutriChat

## Project Overview

In this project, I leveraged the **RAG (Retrieval-Augmented Generation)** concept to build a complete chat pipeline from scratch. Notably, I did not rely on any online RAG frameworks (e.g., Ollama).

### ✨ Key Components

- **Embedding Model**: 
    ```python
    model_name = "all-mpnet-base-v2"
    ```
- **LLM Model**: 
    ```python
    model_name = "google/gemma-2b-it"
    ```
- **Vector Search**: 
    ```python
    Vector Search: FAISS
    ```

### 🚀 Performance Enhancements

In this project, I implemented **flash_attn_2 (Flash Attention)** and **SDPA (Scaled Dot-Product Attention)** to accelerate inference.

- ⚠️ **Note**: Ensure your NVIDIA GPU compute compatibility is 8.0+ for Flash Attention. If not, you’ll need to use SDPA (Single Dot-Product Attention).

### 🔧 Temperature Settings

- **Recommended Temperature**: `0.2`
- This setting depends on the model variant. If you're using:
  - `model: "google/gemma-7b-it"`, you might consider using a slightly higher temperature parameter.
