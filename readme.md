# Gender Abuse detection

**Authors**: Dushyant Singh, Sujal Soni, Mridul Goel\
**Goal**: Detect gendered abuse in English, Hindi, and Tamil using the ULI dataset (7,638–7,914 posts/language).\
**Approach**:

- **Model**: XLM-RoBERTa with BiGRU, multi-head attention, and sigmoid/softmax outputs.
- **Tasks**: Binary classification, transfer learning, multi-class classification (gendered + explicit).
- **Preprocessing**: Cleaned text, normalized emojis, tokenized with XLM-R.\
  **Results**:
- Best F1-scores: Task 1 (0.85, Baseline 2), Task 2 (0.78, Baseline 1), Task 3 (0.43, XLM-BiGRU).
- Challenges: Data sparsity, class imbalance.\
  **Future**: Expand data, refine hyperparameters.


---

### **🚀 How to Run the Project**

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/sujalsoni26/Gendered-Abuse-Detection-in-Indic-Languages.git
   cd Gendered-Abuse-Detection-in-Indic-Languages
   ```

2. **Set Up the Environment**  
   - Create a virtual environment (optional but recommended):  
     ```bash
     python -m venv venv
     source venv/bin/activate  # or venv\Scripts\activate on Windows
     ```
   - Install required dependencies:  
     ```bash
     pip install -r requirements.txt
     ```

3. **Download Pre-trained Embeddings**  
   - Download and place the necessary embedding files (XLM-R) in the appropriate folder as indicated in the notebook.
   

Please download the following pre-trained embeddings before running the models:

#### 📌 GloVe (English)
- **Source**: [GloVe: Global Vectors for Word Representation (Stanford NLP)](https://nlp.stanford.edu/projects/glove/)
- **Recommended File**: `glove.42B.300d.txt` (300-dimensional, 1.9M vocab)

#### 📌 fastText (Hindi and Tamil)
- **Source**: [fastText: Crawl-based Word Vectors](https://fasttext.cc/docs/en/crawl-vectors.html)

- **Hindi**:  
  `cc.hi.300.vec` (300-dimensional)

- **Tamil**:  
  `cc.ta.300.vec` (300-dimensional)

> 💡 Place all downloaded `.vec` or `.txt` files in the `embeddings/` directory or update the paths in the notebook/config accordingly.

4. **Adjust Directory Paths (if needed)**  
   - Modify data and model paths in the notebooks or config files as per your system setup.

5. **Run the Notebook**  
   - Launch the Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Open and execute the desired `.ipynb` file for Task 1, Task 2, or Task 3.

6. **Inferences**
    - Model Checkpoints are saved.
    - Run the appropriate jupyter cells to load the models, dataset and preprocess.
    - Similarly run the appropriate cells for inferencing and evaluation
---