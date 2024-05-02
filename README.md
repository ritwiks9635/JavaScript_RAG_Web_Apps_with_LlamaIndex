# JavaScript_RAG_Web_Apps_with_LlamaIndex
[Complete](https://learn.deeplearning.ai/accomplishments/ac35d85a-7734-4ddc-832a-717c4fac7582?usp=sharing)
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRjWzhICk67AdwBEtCUJXdSnEA5cXnc9SUhgw&usqp=CAU)
People also ask What is LlamaIndex used for? With LlamaIndex you have an easy-to-use data/orchestration framework for ingesting, indexing, and querying your data for building generative AI applications. While we provide a simple example above to get started, the real power of LlamaIndex comes from the ability to build data-driven AI applications.

**LlamaIndex** is an advanced orchestration framework designed to amplify the capabilities of LLMs like GPT-4. While LLMs are inherently powerful, having been trained on vast public datasets, they often lack the means to interact with private or domain-specific data. LlamaIndex bridges this gap, offering a structured way to ingest, organize and harness various data sources — including APIs, databases and PDFs.


By indexing this data into formats optimized for LLMs, LlamaIndex facilitates natural language querying, enabling users to seamlessly converse with their private data without the need to retrain the models. This framework is versatile, catering to both novices with a high-level API for quick setup, and experts seeking in-depth customization through lower-level APIs. In essence, LlamaIndex unlocks the full potential of LLMs, making them more accessible and applicable to individualized data needs.

![](https://docs.llamaindex.ai/en/stable/_static/getting_started/basic_rag.png)
##**How LlamaIndex works**
LlamaIndex serves as a bridge, connecting the powerful capabilities of LLMs with diverse data sources, thereby unlocking a new realm of applications that can leverage the synergy between custom data and advanced language models. By offering tools for data ingestion, indexing and a natural language query interface, LlamaIndex empowers developers and businesses to build robust, data-augmented applications that significantly enhance decision-making and user engagement.



LlamaIndex operates through a systematic workflow that starts with a set of documents. Initially, these documents undergo a load process where they are imported into the system. Post loading, the data is parsed to analyze and structure the content in a comprehensible manner. Once parsed, the information is then indexed for optimal retrieval and storage.


This indexed data is securely stored in a central repository labeled "store". When a user or system wishes to retrieve specific information from this data store, they can initiate a query. In response to the query, the relevant data is extracted and delivered as a response, which might be a set of relevant documents or specific information drawn from them. The entire process showcases how LlamaIndex efficiently manages and retrieves data, ensuring quick and accurate responses to user queries.


Take a look at this enlightening webinar on "How to Build a Gen AI App with LlamaIndex." Dive deep into the world of LLMs and discover the critical role LlamaIndex plays in enhancing their capabilities. This session will not only provide theoretical insights but will also include a hands-on technical demonstration.

**Retrieval Augmented Generation (RAG)** is a groundbreaking framework that enhances Large Language Models (LLMs) by integrating external knowledge sources. RAG overcomes the limitations of LLMs' parametric memory, enabling them to access real-time data, improving contextualization, and providing up-to-date responses.
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTOd1EzkNvVIEErcjLFcF8lt6TSw0WN4SYzLQ&usqp=CAU)

**Prepare data:** Document data is gathered alongside metadata and subjected to initial preprocessing — for example, PII handling (detection, filtering, redaction, substitution). To be used in RAG applications, documents need to be chunked into appropriate lengths based on the choice of embedding model and the downstream LLM application that uses these documents as context.

**Index relevant data:** Produce document embeddings and hydrate a Vector Search index with this data.

**Retrieve relevant data:** Retrieving parts of your data that are relevant to a user's query. That text data is then provided as part of the prompt that is used for the LLM.

**Build LLM applications:** Wrap the components of prompt augmentation and query the LLM into an endpoint. This endpoint can then be exposed to applications such as Q&A chatbots via a simple REST API.
