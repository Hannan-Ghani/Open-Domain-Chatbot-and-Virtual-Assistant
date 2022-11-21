## Open Domain Chatbot and Assistant

Virtual Assistants like alexa and siri cannot hold conversations with a user. They can assist users with several tasks and answer some general questions.

I attempted to create a chatbot which can do both:

1- Have engaging conversations with the user and give human-like responses.
2- Assist the user with several tasks like any other virtual Assistant.

After trying to train different kinds of models mostly seq2seq models on reddit thread dataset, I came across DialoGPT.

DialoGPT is pretrained on millions of conversations from reddit dataset and is able to have engaging conversations with the user. But there is one problem that comes with this. As the model is trained on millions of conversations from millions of different users with different kinds of personalities the responses from chatbot are inconsistent and the chatbot lacks a personality. 

To solve this problem I came across Rick and Morty dataset https://www.kaggle.com/datasets/andradaolteanu/rickmorty-scripts. I removed all other dialogues other than Rick's and finetuned DialoGPT on this dataset. As a result my chatbot got a personality of Rick Sanchez. 

Then I added voice capabilities to the chatbot using a simple python library and gave it some basic functions like playing a music video, sending a message etc. just like any other virtual assistant. 

For future I need to train an intent classifier which will make the chatbot more robust and industrial grade.

I'm still on the lookout for a dataset which can help me create an intent classifier and will be updating this program once I find one
