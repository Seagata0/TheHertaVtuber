# Generative AI Classs's Project - The Herta Vtuber<br>Group 7 (Bojongsantos Oost-indische Compagnie)<br>
![BOC 320](https://github.com/user-attachments/assets/5b04e5ed-6524-4bda-a7d8-6edea5df1511)

# Well, we stir out of the original goal because of... laziness and dissertation paper.


## First Project(Generative AI Prompting) :
- AI Cover Video : https://www.youtube.com/watch?v=4tJADqRNzek (Audio 2:58 (2 Minutes 58 Seconds)) <br>
- Art on Thumbnail : hehe~
- LLM : ChatGPT & DeepSeek
- TTS : Edge-TTS (ja-JP-NanamiNeural)
- Audio Model : Refer to the 2nd Project
- Total Prompt : 41 (Will be used for the second project)
  - Text Prompt : 9 ((https://chatgpt.com/share/67eab298-9814-800b-bb02-8861e6c70c29) & Since Deepseek Cant be shared, the output is shown as "Prompt for TTS" below)
  - Audio Prompt : 24 (Output Can Be checked in /Audio/TTS)

## Second Project (Finetuning) :
### RVC
- RVC Model : [Seagata/TheHerta_RVCModel](https://huggingface.co/Seagata/TheHerta_RVCModel/) (Uploaded there since github can't handle file that is bigger than 25mb) <br>
- Audio source: https://honkai-star-rail.fandom.com/wiki/The_Herta/Voice-Overs/Japanese <br>
- Audio dataset: /VoiceDatasetPreFine-tuning
- Post fine-tuning audio dataset: /TheHertaVoiceDataset
- Google Colab: https://colab.research.google.com/drive/1onf0FOLW46ywWthjMFEdKbh-E70D9v3c?usp=sharing

### LLM
- LLM Model: Not Yet Uploaded (Uploaded there since github can't handle file that is bigger than 25mb) <br>
- Base Model: https://huggingface.co/Sao10K/L3-8B-Stheno-v3.2
- Dataset: /TheHertaLLMDataset
- Dataset Source:
  - https://honkai-star-rail.fandom.com/wiki/The_Herta
  - https://honkai-star-rail.fandom.com/wiki/Herta
  - https://honkai-star-rail.fandom.com/wiki/Aeon
  - https://honkai-star-rail.fandom.com/wiki/Simulated_Universe
- Google Colab: https://colab.research.google.com/drive/1tUYRtgQWdWNnPJXawGNrf5yNWHzT_jux?usp=sharing

## Second Project Implementation :
### RVC
- The Herta AI cover I Like You The Most (https://www.youtube.com/watch?v=4tJADqRNzek)
- I'll add later, though I need to tweak the TTS first

### LLM
- I mean it is a normal gguf LLM, use it wherever you want
- Discord Bot(85% done)
- Telegram Bot (95% done)

## Tools Used:
- Python 3.10.11
- Colab (training)
- https://github.com/rany2/edge-tts (Text To Speech (TTS))
- https://colab.research.google.com/drive/1hmKPNeeReO4NHzOktJFMI2plYKy5F7ZI?usp=sharing (RVC Model Training)
- https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/tree/main (Audio Inference to The Herta)
- ChatGPT(Script Generator)
- Deepseek(Prompting and Script Editing)
- Gemini(to help Sega fixing error)
- Google Translate (Helping Sega to stay sane when translating)
- Audacity (Audio editing & Preprocessing)
- Adobe Photoshop (Image Editing)
- Adobe After Effect (Video editing)
- HandBrake (Video Compression)
- llama.cpp
- koboldcpp
- ollama

## Model Fine Tuning (RVC)
- Audio gathered from honkai-star-rail.fandom.com, consisting of 57 audio file in .ogg format, and later split into 64 .wav file (44100Hz).
- There are 2 models(RMVPE & Harvest) where:
  - RMVPE (750 Epochs)
  - Harvest (300 Epochs)

## Model Fine Tuning (LLM)
- Learning rate: 2e-6
- Epochs: 25 (575 steps)
