# Mainframe Bot

### Motivation
![image](https://github.com/Samueal07/Mainframe-Bot/assets/99087302/5737932a-a2dc-4c21-9ee5-fde8ba086cf1)

A comprehensive GEN AI chatbot which solves your queries related to mainframe!!
![img5](https://github.com/Samueal07/Mainframe-Bot/assets/99087302/0b5ee1a9-5f0b-431c-8068-faa1c32ae5cc)

![img2](https://github.com/Samueal07/Mainframe-Bot/assets/99087302/8c18ae4f-c494-409b-815e-c5e3d4a2241b)
![img1](https://github.com/Samueal07/Mainframe-Bot/assets/99087302/ee9ceb2b-3a5f-443b-8cc8-3bca9398a586)
![img4](https://github.com/Samueal07/Mainframe-Bot/assets/99087302/166ce059-5549-4ec7-909d-735bc13ff451)


### Chat with Mainframe Bot 🚀

- [Huggingface model](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/blob/main/llama-2-7b-chat.ggmlv3.q8_0.bin) as Large Language model
- [LangChain](https://python.langchain.com/docs/get_started/introduction.html) as a Framework for LLM
- [Chainlit](https://docs.chainlit.io/overview) for deploying.
- [GGML](https://github.com/ggerganov/ggml) to run in commodity hardware (cpu)
- [CTransformers](https://github.com/marella/ctransformers) to load the model.

## System Requirements

Python 3.9 or later installed. Earlier versions of python may not compile.

---

## Steps to Replicate

1. Fork this repository and create a codespace in GitHub as I showed you in the youtube video OR Clone it locally.

   ```
   git clone https://github.com/Samueal07/Mainframe-Bot
   cd Mainframe-Bot
   ```

2. Rename example.env to .env with `cp example.env .env`and input the HuggingfaceHub API token as follows. Get HuggingfaceHub API key from this [URL](https://huggingface.co/settings/tokens). You need to create an account in Huggingface webiste if you haven't already.
   ```
   HUGGINGFACEHUB_API_TOKEN=your_huggingface_api_token
   ```
3. Create a virtualenv with conda and activate it. First make sure that you have conda installed. Then run the following command.

   ```
   conda create -n .venv python=3.11 -y && source activate .venv
   ```

4. Run the following command in the terminal to install necessary python packages:

   ```
   pip install -r requirements.txt
   ```

5. Run the following command in your terminal to create the embeddings and store it locally:

   ```
   python3 ingest.py
   ```

6. Run the following command in your terminal to run the app UI:
   ```
   chainlit run main.py -w
   ```
