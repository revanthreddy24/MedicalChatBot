🏥 Medical ChatBot

A Medical Question-Answering Chatbot built using NLP and RAG (Retrieval-Augmented Generation) techniques, trained on The Gale Encyclopedia of Medicine, Second Edition (Volume 1: A–B).

This chatbot is designed to provide structured medical information when given a disease, test, or treatment as input.

✨ Features

Disease Information

Symptoms

Diagnosis

Prevention

Treatment Information

Aftercare

Risks & Complications

Knowledge-Rich Responses

Trained on a comprehensive medical encyclopedia.

Can analyze and provide multiple aspects of medical data.

📂 Project Structure
MedicalChatBot/
│── data/              # Preprocessed medical text dataset
│── notebooks/         # Jupyter notebooks for training & experimentation
│── src/               # Core chatbot implementation
│   ├── model.py       # Model architecture & training code
│   ├── chatbot.py     # Chatbot logic for Q&A
│   └── utils.py       # Helper functions
│── requirements.txt   # Dependencies
│── app.py             # Flask/Streamlit app for chatbot interface
│── README.md          # Project documentation

🚀 Getting Started
1. Clone the Repository
git clone https://github.com/revanthreddy24/MedicalChatBot.git
cd MedicalChatBot

2. Install Dependencies
pip install -r requirements.txt

3. Run the Chatbot

by using the resource folder and trails.ipynb all folders(for now it is not designed using streamlit/flask, will update it very soon)


Then open your browser at http://localhost:5000/
 (Flask) or the provided Streamlit link.

🧠 How It Works

Data Preparation

Extracted text from The Gale Encyclopedia of Medicine (Vol. 1: A–B).

Structured into categories (Symptoms, Diagnosis, Prevention, Aftercare, Risks).

Training

Fine-tuned embedding + retrieval pipeline.

Query → Vector Search → Context Extraction → Response Generation.

Response Generation

If query is about a disease/test → returns symptoms, diagnosis, prevention.

If query is about a treatment → returns aftercare, risks, related info.

🔮 Example Usage

User Input:

What is Malaria?


Bot Output:

Malaria is an infectious disease caused by parasites transmitted through mosquito bites. 
- Symptoms: Fever, chills, sweats, headaches, nausea, and vomiting.  
- Diagnosis: Blood tests to detect parasites.  
- Prevention: Use of mosquito nets, repellents, and preventive medications.  

📌 Future Improvements

Expand training data beyond Vol. 1 (A–B).

Integrate LLM (OpenAI / HuggingFace) for more natural responses.

Add speech-to-text for voice-based interaction.

Deploy as a web app with user-friendly UI.

⚠️ Disclaimer

This chatbot is built for educational and research purposes only.
It should not be used as a substitute for professional medical advice. Always consult a qualified healthcare provider for serious medical concerns.

👨‍💻 Author

Revanth Reddy

Master’s in Computer Science (AI focus)

Passionate about AI, NLP, and Healthcare Applications

GitHub Profile
