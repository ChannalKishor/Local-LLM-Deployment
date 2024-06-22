## Summary

I completed this project by setting up and interacting with large language models (LLMs) on my local machine. First, I downloaded and ran the Llama3 model, ensuring its proper setup and functionality using the `curl` command as instructed. Next, I successfully installed and ran the Mistral model locally and demonstrated its functionality through similar interactions.

Below is the step-by-step guide on how I did this:

**YouTube Demo:** https://www.youtube.com/watch?v=sGaAFlBKTwA
## Step-by-Step Guide

### Step 1: Download Ollama

Ollama is an open-source project that serves as a powerful and user-friendly platform for running LLMs on your local machine.

**Link to download Ollama:** [Ollama Download](http://ollama.com/download)

#### Ollama Commands

 - `Available Commands:   
	 - **serve**       Start ollama  
	 -  **create**      Create model from a Modelfile   
	 - **show**        Show information for a model  
	 - **run**         Run a model   
	 - **pull**        Pull a model from a registry   
	 - **push**        Push a model to a registry   
	 - **list**        List models   
	 - **ps** List running models   
	 - **cp**          Copy a model   
	 - **rm**          Remove a model   
	 - **help**        Help about any command`

### Step 2: Download Llama3 Model

Meta Llama 3, a family of models developed by Meta Inc., is a state-of-the-art model available in both 8B and 70B parameter sizes (pre-trained or instruction-tuned).

**Link to download Llama3:** [Llama3 Download](http://ollama.com/library/llama3)

#### Interacting with Llama3 using Ollama
`ollama run llama3` 

To interact with Llama3 using its API, use the following `curl` command:

`curl http://localhost:11434/api/generate -d "{\"model\": \"llama3\", \"prompt\":\"Why is the sky blue?\"}"` 

> **Note:** I have used a Windows machine, and the commands provided here are for Windows PowerShell.

### Step 3: Download Mistral Model

Similar to Step 2, download the second model, Mistral. Mistral 7B is a 7-billion-parameter language model released by Mistral AI. Mistral 7B is designed to provide both efficiency and high performance for real-world applications.

**Link to download Mistral:** [Mistral Download](http://ollama.com/library/mistral)

#### Interacting with Mistral using Ollama
`ollama run llama3` 

#### Interacting with Mistral using its API

Use the following `curl` command to interact with Mistral:

`curl http://localhost:11434/api/generate -d "{\"model\": \"mistral\", \"prompt\":\"Why is the sky blue?\"}"` 

> **Note:** I have used a Windows machine, and the commands provided here are for Windows PowerShell.
