# nutriChat

## In this project, I leveraged the RAG (retrieval augmented generation) concept to build the full Chat pipeline from scratch. (Didn't use any online RAG frameworks (e.g. ollama))

Embedidng model:
``` Python
model_name = "all-mpnet-base-v2"

```
LLM Model: 
``` Python
model_name = "google/gemma-2b-it
```

```Python
Vector Search : FAISS
```

### In this project I have used flash_attn_2 (Flash attention) and sdpa (scaler dot product attention) to accelerate the inference.
  -> Please make sure that the NVIDIA GPU compute compatibility is 8.0+ otherwise need to use SDPA (single dot prodcut attention).

### Temprature: 0.2 (Recommended), but this is depneds on the model variant you have used. If you have used the  ``` model: "google/gemma-7b-it``` then you can also choose bit higher temprature parameter.


