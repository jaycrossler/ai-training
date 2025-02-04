# AI Playground and training helpers

> Join me in learning hands-on methods for building actual AI systems, integrating local Small Language Models, building AI Agents, and integrating with larger cloud-hosted Large Language Models.  Code is presented to help maximize reuse - so that you can either learn the concepts, or use them within your own applications and systems.

## Welcome to the AI mini "courses"!

All of these examples are living documents of AI techniques - updated so that you can follow along, run code and apps yourself (without having to install software onto your machine), and learn the details of how to employ AI solutions in real world software.  Most are taken from other good notebooks and examples, then tweaked or repaired as code evolves. All credit should go to the original thinkers.

### Python Notebooks that show example code ###

All the items that start with **Notebook** are Python Notebooks that can either be run in [Google Colab](https://colab.research.google.com/) or locally (either by setting up Notebooks locally or copying the Python directly into a local file). If you run them on Google Colab, you need a google colab account (free). When you run a notebook in colab, it spawns a server in the cloud and *usually* assigns GPU time to that server. If you use it heavily, you might need to load $10 or so into your Colab account to pay for more server time, but that shouldn't be necessary if you are just running these modules.

<img src="images/open_in_colab.png" alt="Click the Open in Colab button to load into the cloud" width="400" ></a>
<img src="images/colab_run_block.png" alt="Press the play triangle in each block to run the code within" width="400" ></a><br>
Alternatively, you can install these Notebooks [and run them locally - see instructions here](local_jupyter.md).

### Using Huggingface Spaces ###

HuggingFace is a place to share and research AI models, with a focus on Small Language Models. If you get a free account, you can launch many of the models to test with in "Spaces."
<img src="images/using_huggingface_spaces.png" alt="Run spaces as cloud servers" width="600" ></a>

### Code Notebook Demos/Courses
| | | |
|--|--|--|
|<a href="Exploring_Small_Language_Models.ipynb" target="_blank"><img src="images/DALLE_slm.png" alt="Thumbnail" width="200" ></a>|[Notebook 1: Exploring Small Models](Exploring_Small_Language_Models.ipynb) |Point to a very small (250Mb) model and perform basic queries and AI language tricks on it (like sentence classification or translation). |
|<a href="Ollama%20and%20pydantic.ipynb" target="_blank"><img src="images/ollama_pydantic.png" alt="Thumbnail" width="200" ></a>|[Notebook 2: Ollama and Pydantic](Ollama%20and%20pydantic.ipynb)|Set up a local SLM (or a few of them) using ollama, then use the Pydantic python framework to access it.|
|<a href="Accessing_OpenAI_via_API.ipynb" target="_blank"><img src="images/openai_querying.png" alt="Thumbnail" width="200" ></a>|[Notebook 3: Querying OpenAI remotely](Accessing_OpenAI_via_API.ipynb) |Send queries to OpenAI through python, receive 'structured' responses (to use in apps)<br/>**Requires: OpenAI API Key (not pro account)** |
|<a href="Building%20SmolAgents.ipynb" target="_blank"><img src="images/ai_agent_1.png" alt="Thumbnail" width="200" ></a>|[Notebook 4: Simple AI agents](Building%20SmolAgents.ipynb)|Use the smolagents framework using a SLM to run simple AI agents that write code, create images, and build graphs.|
|<a href="Mistral%20Small%20via%20API.ipynb" target="_blank"><img src="images/ai_crew_rag.png" alt="Thumbnail" width="200" ></a>|[Notebook 5: Exploring the Mistral SLM](Mistral%20Small%20via%20API.ipynb) |Send queries to the highly performant Mistral Small, and test it on common math questions <br/>**Requires: MISTRAL API Key**|
|<a href="Using%20AI%20Agents%20to%20build%20a%20Knowledge%20Graph%20and%20verify%20results.ipynb" target="_blank"><img src="images/python_ai.png" alt="Thumbnail" width="200" ></a>|[Notebook 6: Retrieval-augmented generation (RAG)](Using%20AI%20Agents%20to%20build%20a%20Knowledge%20Graph%20and%20verify%20results.ipynb)| Extract the contents from PDFs, add those to a knowledge graph, then use OpenAI to use that knowledge when answering prompts<br/>**Requires OpenAI API Key**|
|<a href="RAG%20into%20a%20Knowledge%20Graph%20with%20Matryoshka%20Embeddings.ipynb" target="_blank"><img src="images/ai_dolls.png" alt="Thumbnail" width="200" ></a>|[Notebook 7: More efficient RAG](RAG%20into%20a%20Knowledge%20Graph%20with%20Matryoshka%20Embeddings.ipynb)|Use Matryoshka Embeddings to encode knowledge at different levels of complexity, making retrieval faster and a bit better<br/>**Requires: OpenAI API Key and Hugging Face Token**|
|<a href="CrewAI%20Multiple%20Agents%20with%20search.ipynb" target="_blank"><img src="images/ai_crew_1.png" alt="Thumbnail" width="200" ></a>|[Notebook 8: AI Agents that negotiate with each other](CrewAI%20Multiple%20Agents%20with%20search.ipynb)|Use CrewAI with LLaMa 3 running locally (via ollama) to have 4 agents that do research, then negotiate with each other to write a document|
|<a href="CrewAI_Example.ipynb" target="_blank"><img src="images/ai_agent_2.png" alt="Thumbnail" width="200" ></a>|[Notebook 9: AI Agents that search, RAG, and remember](CrewAI_Example.ipynb)|Use CrewAI with OpenAI and a News service to lookup data, store it in a knowledge graph, then answer results<br/>**Requires: OpenAI API Key and newsapi.org Key**|
|<a href="Using-Custom-LLM-Endpoint.ipynb" target="_blank"><img src="images/DALLE_chip.png" alt="Thumbnail" width="200" ></a>|[Notebook 10: Use a custom company model](Using-Custom-LLM-Endpoint.ipynb)|Use LangGraph to build a visual agent workflow with a custom company API<br/>**Requires: Custom company API Key and run within your company (not via colab)**|



### HuggingFace Space Demos/Courses

[Stable Diffusion Image generator:
<img src="images/hf_flux_via_spaces.png" >](https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev)

[Llava image analyzer:
<img src="images/hf_llava.png" >](https://huggingface.co/spaces/badayvedat/LLaVA)

[Non-transformer based Language model:
<img src="images/hf_non_transformer.png" >](https://huggingface.co/spaces/BlinkDL/RWKV-Gradio-2)

[Deepseek when asked about drones:
<img src="images/hf_deepseek_vomiting.png" >](https://huggingface.co/spaces/ruslanmv/DeepSeek-R1-Chatbot)

[Generate 3D models and textures:
<img src="images/hf_3d_model.png" >](https://huggingface.co/spaces/tencent/Hunyuan3D-2)

[Generate sound file with realistic accents:
<img src="images/hf_accents.png" >](https://huggingface.co/spaces/hexgrad/Kokoro-TTS)



---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. Widely recognized as one of the most permissive licenses. Allows users to freely use, modify, and distribute the software with minimal restrictions, only requiring that the original copyright notice be included. 
