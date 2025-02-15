# � Summarization with Transformers (Pegasus on SAMSum Dataset)

## 📝 Description
This Python script demonstrates how to fine-tune the **Pegasus model** for text summarization using the **SAMSum dataset**. The script includes data preprocessing, model training, evaluation, and inference. It leverages the Hugging Face `transformers` library and integrates with the `datasets` library for easy data handling. 🛠️

---

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/navidfalah/summarization-transformers.git
   cd summarization-transformers
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Install additional libraries:
   ```bash
   pip install datasets py7zr evaluate sacrebleu rouge_score
   ```

---

## 🚀 Usage

1. Run the script:
   ```bash
   python summarization_transformers.py
   ```

2. The script will:
   - Load the SAMSum dataset for dialogue summarization.
   - Preprocess the data and tokenize dialogues and summaries.
   - Fine-tune the Pegasus model on the SAMSum dataset.
   - Evaluate the model using ROUGE metrics.
   - Generate summaries for custom dialogues.

---

## 📂 File Structure

```
summarization-transformers/
├── summarization_transformers.py  # Main script
├── README.md                      # This file
├── requirements.txt               # Dependencies
└── data/                          # (Optional) Data folder for local datasets
```

---

## 🧩 Key Features

- **Text Summarization**:
  - Fine-tune the Pegasus model (`google/pegasus-cnn_dailymail`) on the SAMSum dataset.
  - Generate summaries for dialogues using the fine-tuned model.

- **Evaluation**:
  - Use ROUGE metrics to evaluate the quality of generated summaries.
  - Compare model performance before and after fine-tuning.

- **Custom Summarization**:
  - Generate summaries for custom dialogues using the trained model.

- **Visualization**:
  - Plot token length distributions for dialogues and summaries.

---

## 📊 Example Outputs

1. **Summarization Example**:
   - Dialogue: "Thom: Hi guys, have you heard of transformers? Lewis: Yes, I used them recently!"
   - Summary: "Thom and Lewis discuss transformers."

2. **ROUGE Scores**:
   - ROUGE-1: 0.45
   - ROUGE-2: 0.30
   - ROUGE-L: 0.40

3. **Custom Dialogue Summarization**:
   - Input: Custom dialogue about writing a book.
   - Output: "Thom, Lewis, and Leandro plan to write a book about transformers."

---

## 🤖 Models Used

- **Pegasus**: A pre-trained transformer model fine-tuned for summarization tasks.
- **SAMSum Dataset**: A dataset of dialogues and corresponding summaries.

---

## 📈 Performance Metrics

- **ROUGE Scores**:
  - ROUGE-1, ROUGE-2, and ROUGE-L metrics for evaluating summarization quality.

---

## 🛠️ Dependencies

- Python 3.x
- Libraries:
  - `transformers`, `datasets`, `evaluate`
  - `torch`, `matplotlib`, `pandas`
  - `py7zr`, `sacrebleu`, `rouge_score`

---

## 🤝 Contributing

Contributions are welcome! 🎉 Feel free to open an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature`.
3. Commit your changes: `git commit -m "Add your feature"`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a pull request.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Hugging Face for the `transformers` library.
- The SAMSum dataset for providing dialogue summarization data.
- Google Research for the Pegasus model.

---

## 👤 Author

- **Name**: Navid Falah
- **GitHub**: [navidfalah](https://github.com/navidfalah)
- **Email**: navid.falah7@gmail.com
