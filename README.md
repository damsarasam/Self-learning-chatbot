**Generative Chatbot with LSTM**

This repository contains a Python script for building a generative chatbot trained on the Cornell Movie Dialogs Corpus. The chatbot utilizes Long Short-Term Memory (LSTM) networks and skip-gram word embeddings for generating responses in conversational interactions.

### Features:
- **Data Preprocessing**: The script preprocesses the dataset, mapping lines to IDs, extracting conversations, and forming question-answer pairs.
- **Filtering and Tokenization**: Questions and answers are filtered based on length criteria and tokenized using NLTK's word tokenizer.
- **Vocabulary Creation**: A vocabulary is constructed, and encodings and decodings are created for words.
- **Data Transformation**: Training and validation data are transformed into vectors using encodings.
- **Embedding Creation**: Word2Vec skip-gram embeddings are utilized to create embedding matrices for the LSTM model.
- **Model Creation**: An LSTM-based model is built using Keras, with the embedding layer initialized with pre-trained skip-gram embeddings. The model is compiled and trained on the dataset.
- **User Interaction**: Users can interact with the chatbot through a command-line interface. The chatbot predicts responses based on user input, providing an interactive conversation experience.
- **Model Persistence**: The trained model is saved as an HDF5 file for future use.

### Requirements:
- Python 3.x
- NLTK
- Keras
- TensorFlow
- Gensim

### Usage:
1. Clone the repository:
   ```
   git clone https://github.com/your_username/generative-chatbot.git
   ```
2. Navigate to the repository directory:
   ```
   cd generative-chatbot
   ```
3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Run the Python script:
   ```
   python chatbot.py
   ```
5. Interact with the chatbot by entering your queries when prompted.

### Notes:
- Ensure that you have sufficient computational resources for training the model, as it may require significant processing power and memory.
- Experiment with different hyperparameters, such as hidden layer dimensions and training epochs, for optimal performance.
- Feel free to customize the script according to your specific use case and dataset.

### Credits:
This project is based on the Cornell Movie Dialogs Corpus and utilizes concepts from natural language processing and deep learning.

### License:
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Acknowledgments:
Special thanks to the creators of the Cornell Movie Dialogs Corpus for providing the dataset for research purposes.
