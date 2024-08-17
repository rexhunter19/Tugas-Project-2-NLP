# Tugas-Project-2-NLP
Review Summary of BERT Experiment on Liputan6 Dataset for Text Summarization
Objective:
The main goal of this experiment was to evaluate the effectiveness of the BERT model, specifically using the cahya/bert-base-indonesian-1.5G tokenizer, for performing text summarization on the Liputan6 dataset. The dataset was pre-processed, tokenized, and then used to fine-tune the BERT model to generate concise summaries.

Dataset:
The Liputan6 dataset, consisting of Indonesian news articles, was divided into training and evaluation sets. Each article was paired with a corresponding summary, which served as the target output for the model.

Model & Tokenization:
The BERT model, a well-known pre-trained transformer model, was chosen for this task due to its robust performance on various NLP tasks. The cahya/bert-base-indonesian-1.5G tokenizer was employed to handle the Indonesian language text, ensuring that the input articles and summaries were appropriately tokenized for model training.

Experimentation Process:

Data Preparation: The dataset was cleaned and structured, with the articles and summaries concatenated into a format suitable for the model. The data was tokenized using the BERT tokenizer, ensuring consistency in length and structure across the dataset.

Training: The model was fine-tuned on the training set with configurations that included adjusting the maximum lengths for the encoder and decoder, applying a length penalty, and enabling early stopping. The model was trained for three epochs with batch sizes optimized for the available computational resources.

Evaluation: The model was evaluated on a separate validation set. The evaluation focused on metrics like loss and accuracy to determine the model's effectiveness in generating summaries close to the target summaries in the dataset.

Results:
The BERT model, when fine-tuned on the Liputan6 dataset, showed promising results in generating summaries. The evaluation results indicated that the model was able to capture the key points of the articles, producing coherent and contextually accurate summaries. However, the model's performance varied depending on the length and complexity of the input articles.

Visualization:
The evaluation loss was plotted over the epochs to visualize the model's learning progress. The loss steadily decreased, indicating that the model was effectively learning to summarize the articles.

Conclusion:
The BERT model, fine-tuned with the cahya/bert-base-indonesian-1.5G tokenizer, demonstrated a strong capability in text summarization for Indonesian news articles. The results suggest that BERT can be a valuable tool for summarization tasks, though further experimentation with different hyperparameters and model configurations might yield even better performance. Future work could involve exploring more advanced architectures or combining BERT with other models to enhance summarization quality.
