Key Features of this NLP Chatbot:

1.	Dual NLP Engine Support:
•	Primary processing with spaCy (if available) for advanced NLP features
•	Fallback to NLTK when spaCy isn't available

2.	Comprehensive Intent Recognition:
•	Pattern matching for basic queries
•	spaCy NER for entity detection
•	NLTK POS tagging as fallback
•	Combined scoring system for intent matching

3.	Knowledge Domains:
•	Greetings and farewells
•	Time and date queries
•	Mathematical calculations
•	Capabilities explanation
•	Unknown query handling

4.	Conversation Features:
•	Context tracking (last intent, entities)
•	Text preprocessing (lemmatization, stopword removal)
•	Dynamic response generation

5.	Robust Math Processing:
•	Handles basic arithmetic operations
•	Error handling for invalid expressions
•	Clear response formatting

Installation Instructions:
1.	Install required packages:
pip install spacy nltk
python -m spacy download en_core_web_sm
2.	Save the script as nlp_chatbot.py
3.	Run the chatbot:
python nlp_chatbot.py
The chatbot is designed to be extensible - you can easily add new intents and response patterns by expanding the knowledge base dictionary. The dual NLP engine approach makes it resilient to different installation environments.

sample conversation:
Chatbot: Hello! I'm your NLP-powered assistant. Type 'quit' to exit.
You: Hello there
Chatbot: Hi there! What would you like to know?
You: what time is it?
Chatbot: The current time is 14:30.
You: calculate 15 * 3
Chatbot: The result of 15.0 * 3.0 is 45.0.
You: what's the weather
Chatbot: I'm not sure I understand. Could you rephrase that?
You: goodbye
Chatbot: See you later!

