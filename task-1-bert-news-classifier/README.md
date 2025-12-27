## Objective
Fine-tune a BERT-based transformer to classify news articles into four categories.

## Dataset
AG News Dataset (4 classes: World, Sports, Business, Sci/Tech)

## Methodology
- Tokenization using BERT tokenizer
- Fine-tuning bert-base-uncased
- Reduced dataset training due to CPU constraints
- Evaluation using accuracy and macro F1-score

## Results
- Accuracy: 92.25%
- Macro F1-score: 92.34%

## Notes
Training was performed locally on CPU using a reduced subset for efficiency.


“Encoder freezing can be applied to speed up training when only limited compute is available.”