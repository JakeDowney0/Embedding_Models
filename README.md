# Embedding Models

This project implements and compares several classical word embedding techniques:
- Skip-gram (full softmax)
- CBOW (full softmax)
- Skip-gram with Negative Sampling
- GloVe

The learned embeddings are evaluated on a downstream sentiment classification task.

## Results
- Best model: Skip-gram with Negative Sampling
- SST-2 Accuracy: XX.X%  
- Observations: The SGNS and GloVe models significant outperformed the others due to being able to train much quicker without needding to a compute a large softmax (as expected).

## Datasets
- Pretraining: [Wikipedia (Hugging Face)](https://huggingface.co/datasets/wikipedia)  
- Evaluation: [SST-2 (Stanford Sentiment Treebank)](https://huggingface.co/datasets/glue/viewer/sst2)

## How to run

### Option 1: Run on Colab
1. Upload `Embedding_Models.ipynb` to Google Colab  
2. Enable GPU runtime
3. Run all cells

### Option 2: Run Locally
Open the notebook:
    ```bash jupyter notebook Embedding_Models.ipynb
    ```
Then run all cells from top to bottom.
All required dependencies are installed within the notebook.
