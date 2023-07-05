# Using Open Source LLMs on GPU 
In this tutorial we're going to be checking out some of the biggest baddest LLMs...but running them on a GPU!

## See it live and in action 📺
[![Tutorial](https://i.imgur.com/qBoUX8m.jpg)](https://youtu.be/u8vQyTzNGVY 'Tutorial')

# Startup 🚀
1. Create a virtual environment `python -m venv gpullm`
2. Activate it: 
   - Windows:`.\gpullm\Scripts\activate`
   - Mac: `source gpullm/bin/activate`
3. Install PyTorch with CUDA Support 
N.B. I've included the lib in the requirements.txt file but this is latest installer as of creating this readme. 
`pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117`
Download and install CUDA (i've used 11.7 for this tutorial): https://developer.nvidia.com/cuda-11-7-0-download-archive
Download and install the matching cuDNN version ( v8.9.1): https://developer.nvidia.com/rdp/cudnn-archive 
5. Clone this repo `git clone https://github.com/nicknochnack/GPULLM`
6. Go into the directory `cd GPULLM`
7. Install the required dependencies `pip install -r requirements.txt`
8. Update the path of the models in line 9 of `app.py` and line 5 of `app-chain.py`
9.  Start the python agent app by running `streamlit run app.py` or the chain app by running `streamlit run app-chain.py`  
10. Go back to my YouTube channel and like and subscribe 😉...no seriously...please! lol 
11. The comparison app can be started by running `streamlit run app-comparison.py` before you do that though, update the base ggml download path in line 16, e.g. `BASE_PATH = 'C:/Users/User/AppData/Local/nomic.ai/GPT4All/'` and openAI api key on line 18


# Other References 🔗
<p>-<a href="https://pytorch.org/get-started/locally/">PyTorch Installation</a>:main guide leveraged to handle GPU support.</p>
<p>-<a href="https://python.langchain.com/en/latest/modules/models/llms/integrations/huggingface_pipelines.html">Langchain HF Pipelines</a>:the HF Pipelines class is used in order to pass the local LLM to a chain.</p>

# Who, When, Why?
👨🏾‍💻 Author: Nick Renotte <br />
📅 Version: 1.x<br />
📜 License: This project is licensed under the MIT License </br>

