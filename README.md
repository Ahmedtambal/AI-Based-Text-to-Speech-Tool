# AI-Based Text-to-Speech Tool

![image](https://github.com/user-attachments/assets/7e83c5b7-3d96-4252-a92a-457d979d56d5)


This repository contains a Text-to-Speech (TTS) tool that leverages the BARK model by Suno for generating natural-sounding audio from text input. The tool provides multiple voices across different languages, allowing users to select their preferred voice characteristics.

## **Features**
- **Multiple Voices**: Choose between male and female voices in English and Chinese.
- **Flexible Voice Control**: Select your preferred voice style for a tailored audio experience.
- **Web-Based Interface**: Easy-to-use Gradio interface for user interaction.

---

## **Installation and Setup**

### **Dependencies**

Install the necessary dependencies by running:

```bash
pip install gradio transformers torch librosa soundfile werkzeug
```
### **Main Libraries**
- **Gradio**: For creating a web interface to interact with the model.
- **Transformers**: To load the BARK model and process text input.
- **Torch**: For model processing and inference.
- **Librosa & Soundfile**: For audio processing and saving.
- **Werkzeug:** For handling server interactions securely.

### **Other Imports**
- numpy, scipy, and os are also used to handle audio arrays and file saving.

---

### **Running the Tool**
- Load the Tool: Run all cells in the Jupyter Notebook to set up configurations, load models, and initialize functions.
- Enter Text and Select Voice: Type your desired text in the text box, choose a voice from the provided options, and press Submit to generate speech.
- Playback: The generated audio will appear as a downloadable file or can be played directly within the Gradio interface.

---

### **About the BARK Model**
The BARK model by Suno is a powerful Text-to-Speech (TTS) model designed to create high-quality, lifelike audio. Key aspects of the model include:

- Multi-language Support: BARK can generate speech in multiple languages, making it adaptable for various global use cases.
- Voice Diversity: BARK enables customization of voice style, gender, and tone, allowing for more personalized audio outputs.
- Efficient Processing: Utilizing transformer-based architecture, BARK is optimized for generating natural-sounding speech efficiently.

### **Limitations**
- Length Constraints: Due to its transformer structure, BARK has a maximum input length. For longer texts, you’ll need to split the input into shorter sentences.
- Noise at Sentence Boundaries: In some cases, the model may add slight noise or artifacts between sentences, especially if sentences are short or abrupt.
- Handling Parentheses: Content in parentheses may sometimes be omitted in the audio output. If this happens, rephrase the text using commas or other punctuation.
- It can take up to 1 minute to generate an audio depending on the length of the text.

### **Pros**
- High-Quality Audio: BARK produces clear, expressive audio with lifelike intonation.
- Customizable Voices: Multiple voice presets enable a range of audio styles and characteristics.
- Open-Source Flexibility: BARK is open-source and easily customizable, with an active community for support.

---

### **Usage Guide**
- Enter Text: Write or paste the text you want to convert into speech in the designated text box (up to around 1,000 characters for optimal performance).
- Select a Speaker: Choose between different speaker options (e.g., Male/Female in English or Chinese) for the audio generation.
- Generate Audio: Press Submit to start the text-to-speech conversion.
- Listen and Download: Once generated, you can listen to the audio directly in the Gradio interface or download it as a .wav file.

---

### **Limitations and Further Development**
The tool is ideal for basic text-to-speech applications but may need further optimizations for high-performance requirements or extended use cases. Future improvements could focus on reducing noise artifacts, handling longer texts more effectively, and expanding voice options.
Feel free to experiment with the code and modify voice settings or model configurations to enhance the tool’s performance and capabilities!



