# 🚀 Multilingual Customer Support Chatbot
    This project implements a Multilingual Customer Support Chatbot using machine learning and natural language processing (NLP). The chatbot can detect user intent, extract entities, analyze sentiment, and respond in multiple languages.

# 📜 Features

    🔍 Intent Detection: Recognizes user intent using logistic regression.
    🌐 Multilingual Support: Automatically detects and translates non-English inputs.
    📝 Entity Extraction: Identifies key entities from user queries.
    😊 Sentiment Analysis: Determines if user sentiment is positive, negative, or neutral.
    📊 Confidence Filtering: Only responds when intent confidence is above 70%.
    🖨️ Interactive CLI: Engage with the chatbot through the terminal.

# 🎥 Example Conversation
    User Input (es): ¿Cómo cancelo mi pedido?
    Response: Intención detectada: cancel_order. ¿Cómo puedo ayudarte más?

    User Input (fr): Quelle est la politique de remboursement ?
    Response: Intention détectée: refund_policy. Je peux vous aider avec d'autres questions?

# 🛠️ Installation
    Ensure you have Python 3.8+ and the required packages installed:

    # Create virtual environment (optional but recommended)
      python -m venv chatbot-env
      source chatbot-env/bin/activate  # On Windows: chatbot-env\Scripts\activate

    # Install dependencies
      pip install pandas numpy nltk googletrans==4.0.0-rc1 textblob spacy scikit-learn

    # Download NLTK and spaCy resources
      python -m nltk.downloader wordnet
      python -m spacy download en_core_web_sm

# 📂 Dataset

    Ensure the dataset Bitext_Sample_Customer_Support_Training_Dataset_27K_responses-v11.csv exists in the project folder with columns:
    instruction (User queries)
    intent (Corresponding intents)

# 🚀 Running the Chatbot

    Run the chatbot script:
    you can convert the into python chatbot.py because its on ipynb

# ⚙️ Project Structure

    📦 Multilingual_Ai_Chatbot
    ├─ 📄 Multilingual AI Chatbot.ipynb  # Main chatbot code (Jupyter Notebook)
    ├─ 📄 Bitext_Sample_Customer_Support_Training_Dataset_27K_responses-v11.csv  # Dataset
    ├─ 📄 README.md                      # Project documentation
    └─ 📜 LICENSE                       # License details
    
# 📊 Usage
    Start the chatbot:
      python chatbot.py

    Example Queries:
      "How do I track my order?"
      "¿Cuál es el costo de envío?"
      "What is your refund policy?"

# 📝 Configuration
    To adjust confidence thresholds, modify this line in chatbot.py:
    if confidence < 0.7:

# 🤝 Contributing
    Feel free to submit pull requests or report issues. Ensure code follows PEP8 standards.

# 🛡️ License
    This project is licensed under the MIT License.

# 🙌 Acknowledgments
    Special thanks to the open-source community for tools like NLTK, spaCy, and Google Translate API.
