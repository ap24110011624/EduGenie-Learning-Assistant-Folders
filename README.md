# 🧠 EduGenie: Emotion Detection & Learning Support Engine

An AI-powered web application that detects students' emotions from text and provides personalized learning guidance using deep learning models and Google Gemini AI.
---

## 📌 Project Overview

Students often experience emotions such as confusion, frustration, curiosity, or confidence while learning. This project analyzes a student's written learning problem, detects the underlying emotion using machine learning models, and provides personalized recommendations and AI-generated guidance.

The application combines deep learning with Generative AI to create an intelligent learning support system.

---

## 🎯 Objectives

- Detect student emotions from learning-related text.
- Compare emotion prediction using BiLSTM and BERT.
- Provide personalized learning recommendations.
- Generate empathetic AI guidance using Google Gemini.
- Maintain analysis history for continuous learning.
- Visualize analytics through an interactive dashboard.

---

## ✨ Features

- 🧠 **Emotion Detection using BiLSTM**: Tailored Recurrent Neural Network model optimized for learning context.
- 🤖 **Emotion Detection using BERT**: High-accuracy Transformer model for text analysis.
- 💬 **AI Learning Guidance using Google Gemini**: Custom Gemini prompt engineering for educational support.
- 📚 **Subject-wise Learning Support**: Tailored recommendations for Math, Science, Programming, and more.
- 📈 **Emotion Confidence Score**: Probability distributions of detected student sentiment.
- 📊 **Analytics Dashboard**: Performance metrics and statistics for learning patterns.
- 📜 **Session History**: Localized history tracking using secure storage.
- 📄 **Downloadable Analysis Report**: PDF generation for offline progress review.
- 🌐 **Interactive Streamlit Web Application**: Clean, modern, responsive UI design.

---

## 🛠️ Technologies Used

### Programming Language
- Python

### Machine Learning & AI
- TensorFlow / Keras
- PyTorch
- Hugging Face Transformers
- Google Gemini API

### Web Framework
- Streamlit

### Data Processing & Visualization
- NumPy, Pandas, Scikit-learn
- Plotly

---

## 📂 Project Structure

This repository follows the **SmartBridge / SkillWallet Capstone Repository** design standard:

```
EduGenie-Learning-Assistant/
├── 1_Brainstorming_and_Ideation/   # Problem definitions, brainstorming notes, empathy maps
├── 2_Requirement_Analysis/         # Data flow diagrams, stack selection, user journeys
├── 3_Project_Design_Phase/          # Solution architecture, interface design mockups
├── 4_Project_Planning_Phase/        # Project plans, scheduling documents
├── 5_Project_Development_Phase/     # Application source code
│   ├── backend/                     # Backend components placeholder
│   ├── frontend/                    # Frontend components placeholder
│   ├── templates/                   # UI HTML templates placeholder
│   ├── static/                      # Static resources and assets placeholder
│   ├── tests/                       # Unit/integration test suites placeholder
│   ├── history/                     # User session data history
│   ├── pages/                       # Multi-page Streamlit dashboards
│   ├── app.py                       # Main application entry point
│   ├── config.py                    # Project paths and configuration settings
│   ├── emotion_detector.py          # BiLSTM and BERT prediction logic
│   ├── gemini_service.py            # Google Gemini AI connection and prompting
│   ├── preprocessing.py             # NLP text cleanup and preprocessing
│   ├── recommendation_engine.py     # Rule-based and AI recommendations
│   ├── requirements.txt             # Project requirements and dependencies
│   ├── utils.py                     # Helper functions
│   └── Dockerfile                   # Docker container configuration
├── 6_Project_Testing/               # Performance and unit test documentation
├── 7_Project_Documentation/         # Executive summary and technical manuals
├── 8_Project_Demonstration/         # Video links, slides, and demo collateral
├── LICENSE                          # MIT License
└── README.md                        # Documentation entry point
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone <repository-url>
cd EduGenie-Learning-Assistant
```

### 2. Set up Virtual Environment
```bash
python -m venv venv
```

#### Activate the environment:
- **Windows**:
  ```bash
  venv\Scripts\activate
  ```
- **Linux / macOS**:
  ```bash
  source venv/bin/activate
  ```

### 3. Install dependencies
```bash
pip install -r 5_Project_Development_Phase/requirements.txt
```

---

## ▶️ Running the Application

Navigate to the project development directory:
```bash
cd 5_Project_Development_Phase
```

Run the Streamlit application:
```bash
streamlit run app.py
```

The application will launch locally at `http://localhost:8501`.

---

## 🐳 Running with Docker

You can build and run the application container using the provided Dockerfile.

### 1. Build the Docker Image
```bash
docker build -t edugenie-app -f 5_Project_Development_Phase/Dockerfile 5_Project_Development_Phase/
```

### 2. Run the Container
```bash
docker run -d -p 8501:8501 --env GEMINI_API_KEY="your-api-key" edugenie-app
```

---

## 🧠 Application Workflow

1. **Enter Problem**: The user enters their current learning problem/text.
2. **Select Subject**: The user picks the subject they are working on (e.g., Mathematics, Coding).
3. **Choose Model**: Select the model for classification (BiLSTM or BERT).
4. **Analyze Emotion**: The application preprocesses the text and runs predictions.
5. **Get Advice**: The system generates specific learning advice and calls Gemini to create empathetic guidance.
6. **Save & Export**: Save session stats and download the report.

---

## 👨‍💻 Developed By

**EduGenie Team**  
*SkillWallet / SmartBridge Capstone Project*

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.