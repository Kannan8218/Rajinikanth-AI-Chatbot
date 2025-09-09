# Rajinikanth Chatbot

A conversational AI chatbot that mimics Superstar **Rajinikanth’s** personality using **Streamlit**, **Keras**, **NLTK**, and **scikit-learn**. The chatbot responds in **Thanglish** (a mix of Tamil and English) with short, direct, and respectful replies in Rajinikanth’s unique style. It includes avatars, GIFs, session management, and exportable chat history.

---

## 📦 Project Structure

```
├── rajini_data.json           # Dataset with intents, patterns, and responses
├── Rajini_display.py          # Streamlit app for the user interface and session handling
├── Rajini_NLP.py              # Machine learning pipeline for intent classification
├── style.css                  # Styling for the app interface
├── image/                     # Contains Rajinikanth's avatars and related images
├── gif/                       # Contains GIF animations of famous Rajinikanth dialogs
├── about.txt                  # Text file with information about the chatbot
├── requirements.txt           # Python dependencies for easy setup
└── README.md                  # This documentation file
```

---

## 🚀 Features

✔ Chat with Rajinikanth in a conversational style  
✔ Context-aware responses based on past interactions  
✔ Personalized avatar and dialog animations  
✔ Export chat history as PDF  
✔ Custom UI with adjustable colors and fonts  
✔ Local machine learning model using intent classification  
✔ Optionally integrated with Google Gemini API for advanced language models

---

## 📂 Dataset – `rajini_data.json`

- Contains categorized intents like:
  - Greetings
  - Personal information (name, family, birthdate)
  - Career details (movies, awards, acting start)
  - Fun and entertainment queries  
- Each intent includes patterns (example questions) and responses (replies).

---

## 🧠 Machine Learning – `Rajini_NLP.py`

- Text preprocessing using `nltk` and regular expressions
- Feature extraction using TF-IDF for both words and characters
- Intent classification with a feedforward neural network
- Model evaluation using accuracy, precision, recall, and F1-score
- Handles data imbalance with class weighting
- Saves vectorizers and models for inference

---

## 🖥 User Interface – `Rajini_display.py`

- Built with Streamlit for real-time interaction
- Displays chat history with avatars and animations
- Uses session state to persist data during interactions
- Provides export functionality to save conversations as PDF
- Customizable appearance with CSS styling
- Supports text input and optionally integrates Gemini API

---

## 📥 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/rajinikanth-chatbot.git
   cd rajinikanth-chatbot
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download necessary NLTK packages:
   ```bash
   python -m nltk.downloader punkt wordnet omw-1.4
   ```

4. Run the Streamlit app:
   ```bash
   streamlit run Rajini_display.py
   ```

---

## ⚙ Requirements (`requirements.txt`)

```txt
streamlit
nltk
numpy
scikit-learn
tensorflow
keras
reportlab
scipy
google-generativeai
```

You can create this file with the above content to ensure easy environment setup.

---

## 📂 How It Works

1. User types a query into the chat interface.
2. The input is preprocessed and matched against intents using the trained model.
3. The chatbot selects the best response from the dataset.
4. The UI displays the reply with avatars and animations.
5. The conversation is saved and can be exported as a PDF.

---

## 📈 Future Improvements

- Add voice recognition and text-to-speech
- Enhance dataset with more conversational patterns
- Use transformer models for advanced natural language understanding
- Implement personalized responses with user profiles
- Deploy on cloud platforms with API support

---

## 📄 License

This project is **proprietary**.  
You are **not permitted** to use, modify, or distribute the code or dataset without prior written consent from the author/maintainer.  
All rights reserved.

---

## 📧 Contact

For questions or collaboration, feel free to open an issue or contact the maintainer.

---

Enjoy chatting with Rajinikanth! 🎬✨
