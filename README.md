# WIKI-GOD_BOT
God Bot: AI-Powered Wikipedia Question Answering System

God Bot is an advanced, interactive question-answering system that leverages the vast knowledge base of Wikipedia to provide informative responses to user queries. By combining speech recognition, natural language processing, and information retrieval techniques, God Bot offers a unique and engaging way to explore and learn from Wikipedia content.

Table of Contents

Features
How It Works
Technical Details
Dependencies
Installation
Usage
Limitations and Considerations
Future Improvements
Contributing
Features

Speech-to-Text Input: Users can interact with the system using voice commands, making it accessible and user-friendly.
Wikipedia Integration: Dynamically fetches and processes content from any Wikipedia article specified by the user.
Natural Language Processing: Utilizes NLTK (Natural Language Toolkit) for advanced text processing, including tokenization and lemmatization.
TF-IDF Vectorization: Implements Term Frequency-Inverse Document Frequency vectorization for effective text representation.
Cosine Similarity Matching: Employs cosine similarity to find the most relevant sentences that answer user queries.
Interactive Loop: Provides a continuous question-answering experience until the user decides to stop.
How It Works

Article Selection: The user specifies a Wikipedia article of interest.
Content Retrieval: God Bot fetches the full content of the specified Wikipedia page.
Query Input: Users can ask questions about the topic verbally.
Speech Recognition: The system converts speech to text using Google's speech recognition API.
Text Processing: Both the question and the Wikipedia content are processed using NLP techniques.
Answer Retrieval: The system identifies the most relevant sentence from the article as the answer.
Response: The answer is displayed to the user.
Continuation: The process repeats for new questions until the user ends the session.
Technical Details

Natural Language Processing

Tokenization: Breaks down the text into individual sentences and words.
Lemmatization: Reduces words to their base or dictionary form, improving matching accuracy.
Part-of-Speech Tagging: Identifies word types (nouns, verbs, etc.) to enhance lemmatization.
Information Retrieval

TF-IDF Vectorization: Converts text to numerical vectors, emphasizing important words.
Cosine Similarity: Measures the similarity between the question vector and sentence vectors from the article.
Speech Recognition

Utilizes Google's speech recognition API for accurate transcription of user queries.
Dependencies

NLTK: For natural language processing tasks
scikit-learn: For TF-IDF vectorization and cosine similarity computation
Wikipedia-API: To fetch Wikipedia article content
SpeechRecognition: For converting speech to text
PyAudio: For capturing audio input (required by SpeechRecognition)
Installation

Install the required packages:

pip install nltk scikit-learn wikipedia-api SpeechRecognition pyaudio
Download necessary NLTK data:

import nltk
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')
nltk.download('wordnet')
Usage

Run the Jupyter notebook:

jupyter notebook "god bot.ipynb"
Execute the cells in order.

When prompted, enter the name of a Wikipedia article you want to explore.

Ask questions verbally when prompted with "Say something!"

To end the session, say "stop" or type "stop" when prompted for a question.

Limitations and Considerations

The accuracy of answers depends on the content available in the Wikipedia article and the relevance of the question.
Speech recognition may not work perfectly in noisy environments or with certain accents.
The system provides single-sentence answers, which may not always capture the full context.
It doesn't understand context from previous questions in the conversation.
Future Improvements

Implement multi-sentence answer generation for more comprehensive responses.
Add support for multiple languages in both input and output.
Introduce a caching mechanism to improve response time for repeated queries.
Develop a graphical user interface for easier interaction.
Implement error handling for network issues or unavailable Wikipedia pages.
Integrate with a more robust knowledge base beyond Wikipedia.
Contributing

Contributions to God Bot are welcome! Please feel free to submit pull requests, report bugs, or suggest new features through the GitHub issue tracker.

God Bot is an educational project and is not affiliated with or endorsed by the Wikimedia Foundation.
