ChatBot using PyTorch
Overview
This project is a simple conversational chatbot built using PyTorch. It leverages a pre-trained neural network to classify user input into predefined intents and responds accordingly. The chatbot uses Natural Language Processing (NLP) techniques like tokenization, stemming, and a bag-of-words approach to process text.

Features
Deep Learning: Utilizes a multi-layer neural network built with PyTorch.
NLP Techniques: Includes tokenization, stemming, and bag-of-words to process input text.
Custom Intents: Customizable intents file (intents.json) to modify the chatbot's responses.
Interactive Conversations: Engage with users in real-time through the command line.
Project Structure
bash
Copy code
├── data.pth             # Trained model parameters
├── intents.json         # The dataset of patterns, responses, and intents
├── model.py             # Neural network model definition
├── nltk_utils.py        # NLP helper functions (tokenization, stemming, bag-of-words)
├── train.py             # Script to train the chatbot model
└── chat.py              # Script to interact with the trained chatbot
Prerequisites
To run this project, you will need the following:

Python 3.x
PyTorch library
nltk library (for NLP tasks)
Installation
Clone the repository:
bash
Copy code
git clone https://github.com/MMKCODE45/chatbot-pytorch.git
Install the required libraries:
bash
Copy code
pip install torch nltk
Download NLTK data (if not already installed):
python
Copy code
import nltk
nltk.download('punkt')
Training the Model
Before interacting with the chatbot, you can train the model using the train.py script:

Modify the intents.json file to include your own intents, patterns, and responses.
Run the training script:
bash
Copy code
python train.py
This will train the chatbot and save the model parameters in data.pth.
Running the Chatbot
Once the model is trained, you can interact with the chatbot using the chat.py script:

bash
Copy code
python chat.py
Type your questions and chat with the bot. To exit, simply type quit.

Example Conversation
vbnet
Copy code
You: Hi
Bot: Hello, how can I assist you?

You: What services do you provide?
Bot: I offer general customer support. How can I help you today?

You: quit
