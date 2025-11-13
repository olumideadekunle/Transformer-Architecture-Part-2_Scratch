This project implements a Transformer-based sequence-to-sequence model from scratch for machine translation, specifically translating English sentences to French. The implementation showcases the core components of the Transformer architecture, including tokenization, embedding, positional encoding, multi-head attention, and feed-forward networks.


# Transformer-Architecture-Part-2_Scratch
# Transformer Model for Machine Translation (English to French)  This project implements a Transformer-based sequence-to-sequence model from scratch for machine translation
# Transformer Model for Machine Translation (English to French)


## Key Features:

- **Data Preparation**: Downloads and processes an English-French parallel corpus (`fra.txt`) from [manythings.org](http://www.manythings.org/anki/fra-eng.zip).
- **Custom Tokenization and Vocabulary**: Includes a custom tokenizer and vocabulary builder to handle sentence encoding and decoding.
- **PyTorch Dataset and DataLoader**: Manages data loading and batching with custom `TranslationDataset` and `collate_fn` for padding.
- **Transformer Architecture**: Implements a `TransformerSeq2Seq` model using PyTorch's `nn.Transformer` module, along with custom embedding and positional encoding layers.
- **Training and Validation**: Trains the model over multiple epochs with Adam optimizer and CrossEntropyLoss, tracking training and validation loss/accuracy.
- **Performance Visualization**: Plots training and validation loss and accuracy curves to monitor model performance.
- **BLEU Score Evaluation**: Evaluates the model's translation quality using the BLEU score metric.

## How to Use:

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```
2. **Install Dependencies**:
   ```bash
   pip install torch pandas matplotlib nltk tqdm
   ```
3. **Run the Jupyter Notebook / Colab**:
   Open and run the provided notebook, which will guide you through data download, preprocessing, model training, and evaluation.

## Results:

The project demonstrates the feasibility of building and training a Transformer model for a basic machine translation task. The loss and accuracy curves provide insights into the training process, and the BLEU score quantifies the translation quality (though it might require further optimization for higher scores).
