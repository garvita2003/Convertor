# Convertor Suite (Text, Image, and Speech) 🔁

## 📌 Introduction

Convertor is a Python-based mini AI toolkit that demonstrates multiple conversion workflows in one project:

- ✅ Text-to-Image generation using Stable Diffusion
- ✅ Multilingual Text-to-Image with translation to English
- ✅ Image-to-Text caption generation
- ✅ Speech-to-Text with Text-to-Speech playback

The project combines notebook-based GenAI experiments with a standalone Python script for live microphone input processing.

---

## 🔄 Process / Flow

1. User selects a conversion workflow (text, multilingual text, image, or speech).
2. For text-to-image, prompt is sent to Stable Diffusion pipeline.
3. For multilingual text-to-image, input text is translated to English first, then image is generated.
4. For image-to-text, an image is passed through a vision-captioning model to generate a description.
5. For speech-to-text, microphone audio is recognized with Google Speech Recognition.
6. Recognized text is spoken back using text-to-speech engine.

---

## 🛠️ Technology Used

| Component | Technology |
|-----------|-----------|
| Language | Python |
| Notebook Workflow | Jupyter Notebook |
| Text-to-Image | diffusers + Stable Diffusion (`stabilityai/stable-diffusion-2`) |
| Translation | googletrans |
| Image Captioning | Transformers (`nlpconnect/vit-gpt2-image-captioning`) |
| Speech Recognition | speechrecognition (Google recognizer) |
| Text-to-Speech | pyttsx3 |
| Audio Input | PyAudio + Microphone |
| Core ML Runtime | torch |

---

## 🎓 Skills Gained

### Generative AI Pipelines

- ✅ Building text-to-image generation workflows with Hugging Face Diffusers
- ✅ Integrating multilingual preprocessing before generation
- ✅ Managing model setup and inference parameters in notebook experiments

### Speech and Audio Processing

- ✅ Capturing real-time microphone input in Python
- ✅ Converting speech to text using recognizer APIs
- ✅ Replaying recognized content using text-to-speech

### Multimodal AI Integration

- ✅ Combining NLP, vision, and audio workflows in a single project
- ✅ Working with pretrained transformer models for image captioning
- ✅ Structuring quick prototypes for end-to-end AI conversions

---

## 📂 Project Structure

```text
Convertor-main/
├── README.md                  # Project documentation
├── TextToImage.ipynb          # Notebook: text-to-image, multilingual generation, and image captioning
└── SpeechToTextAudio.py       # Script: live speech-to-text with text-to-speech output
```

---

## 📸 Demonstration

1. Text-To-Image using GenAI
![Screenshot 2024-12-28 202533](https://github.com/user-attachments/assets/2e223a59-ef3d-4a47-9cf7-e035ecb08b74)

2. Multilingual Text-To-Image
![Screenshot 2024-12-28 202556](https://github.com/user-attachments/assets/359e59cf-154f-4ea3-b477-177a7f57be30)

3. Image-To-Text
![Screenshot 2024-12-28 202613](https://github.com/user-attachments/assets/3d94cfc8-49ff-4539-bd35-fda09475a20d)

4. Speech-To-Text and Audio
![Screenshot 2024-12-28 204732](https://github.com/user-attachments/assets/cc78fc8b-7406-499f-be14-4ec23ea5d855)

---

## ⚙️ Setup Instructions

### ✅ Prerequisites

- ✅ Python 3.8+
- ✅ Jupyter Notebook / JupyterLab (for `TextToImage.ipynb`)
- ✅ Hugging Face account and access token for Stable Diffusion model usage
- ✅ Working microphone device (for speech workflow)

### 📦 Installation

Install core dependencies:

```bash
pip install torch diffusers transformers googletrans==3.1.0a0 pillow speechrecognition pyaudio pyttsx3
```

### ▶️ Run

1. Open and run notebook workflows:

```bash
jupyter notebook TextToImage.ipynb
```

2. Run speech-to-text + text-to-speech script:

```bash
python SpeechToTextAudio.py
```
