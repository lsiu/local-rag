# RAG working with local LLM using llama.cpp

Reference web pages:

* [DeepLearning.AI's LangChain Chat with Your Data](https://learn.deeplearning.ai/courses/langchain-chat-with-your-data)
* I end up using [bartowski/Meta-Llama-3.1-8B-Instruct-GGUF available on huggingface](https://huggingface.co/bartowski/Meta-Llama-3.1-8B-Instruct-GGUF/tree/main) for local model. Specifically the `Meta-Llama-3.1-8B-Instruct-Q6_K_L.gguf` one.
* I also tried using [langchain's llama-cpp](https://python.langchain.com/v0.2/docs/integrations/llms/llamacpp/)
* Backend we used [Chroma vector store and use the langchain abstraction](https://python.langchain.com/v0.2/docs/integrations/vectorstores/chroma/). I also tried milvus, but it's local test version does not work on Windows.
* Using [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) with the `create_chat_completion` feature end up giving me a good enough result for query data from documents 