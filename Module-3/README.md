# BERT-Based Sentiment Analysis on IMDB Dataset

## Module 3: Fine-Tuning Pre-trained Models for Text Classification

**Author:** Marco Gonzalez  
**Course:** AAI-520 Applied Artificial Intelligence  
**Assignment:** BERT Sentiment Analysis Implementation  

---

## Project Overview

This project implements BERT-based sentiment analysis on the IMDB movie review dataset. The implementation demonstrates fine-tuning a pre-trained transformer model for binary text classification, covering the complete machine learning pipeline from data preprocessing to model evaluation.

## Key Features

- **BERT Tokenization**: Proper text preprocessing using BERT tokenizer
- **Fine-Tuning Implementation**: Transfer learning with pre-trained BERT model
- **Comprehensive Evaluation**: Multiple metrics including accuracy, precision, recall, F1-score
- **Practical Application**: Sentiment prediction on sample movie reviews
- **Academic Presentation**: Clean, professional code without excessive complexity

## Technical Implementation

### Data Processing
- IMDB dataset with 50,000 movie reviews (subset of 5,000 used for efficiency)
- Binary sentiment classification (positive/negative)
- BERT tokenization with appropriate padding and truncation
- Train/test split with stratification

### Model Architecture
- **Base Model**: BERT-base-uncased from Hugging Face Transformers
- **Task Adaptation**: Sequence classification head for binary sentiment
- **Parameters**: ~110M trainable parameters
- **Optimization**: Adam optimizer with learning rate scheduling

### Training Configuration
- **Epochs**: 2 (reduced for practical training time)
- **Batch Size**: 16
- **Max Sequence Length**: 256 tokens
- **Hardware**: CPU/GPU compatible implementation

## Results and Performance

The fine-tuned BERT model achieves strong performance on sentiment analysis:

- **Accuracy**: High classification accuracy on test set
- **Precision/Recall**: Balanced performance across sentiment classes
- **F1-Score**: Strong harmonic mean of precision and recall
- **Confusion Matrix**: Clear visualization of classification performance

## File Structure

```
Module-3/
├── 3-1-BERT-Sentiment-Analysis-Marco-Gonzalez.ipynb  # Main analysis notebook
├── IMDB Dataset.csv                                  # Movie review dataset
├── requirements.txt                                  # Python dependencies
└── README.md                                         # This documentation
```

## Installation and Setup

### Prerequisites
- Python 3.8 or higher
- CUDA-compatible GPU (optional, but recommended)
- Minimum 8GB RAM (16GB recommended)

### Dependencies Installation
```bash
pip install -r requirements.txt
```

### Key Libraries
- `transformers`: Hugging Face Transformers library
- `torch`: PyTorch deep learning framework
- `scikit-learn`: Evaluation metrics and utilities
- `pandas`: Data manipulation and analysis
- `numpy`: Numerical computing
- `matplotlib/seaborn`: Data visualization

## Usage Instructions

1. **Environment Setup**:
   ```bash
   cd Module-3
   pip install -r requirements.txt
   ```

2. **Launch Notebook**:
   ```bash
   jupyter notebook 3-1-BERT-Sentiment-Analysis-Marco-Gonzalez.ipynb
   ```

3. **Execute Cells**: Run cells sequentially for complete analysis

4. **Training Time**: Expect 10-30 minutes depending on hardware

## Implementation Highlights

### BERT Tokenization
- Proper handling of special tokens ([CLS], [SEP])
- Attention mask generation for variable-length sequences
- Truncation and padding for consistent input dimensions

### Fine-Tuning Process
- Pre-trained weights initialization from BERT-base-uncased
- Task-specific classification head training
- Gradient-based optimization with appropriate learning rates
- Evaluation during training for model selection

### Model Evaluation
- Comprehensive metrics calculation
- Confusion matrix visualization
- Per-class performance analysis
- Sample prediction demonstrations

### Prediction Interface
- Function for sentiment prediction on new text
- Confidence score calculation
- Practical examples with movie reviews

## Academic Considerations

### Methodology
- Follows standard transfer learning practices
- Implements proper train/validation/test splits
- Uses appropriate evaluation metrics for binary classification
- Maintains reproducibility with random seed setting

### Code Quality
- Clean, well-documented implementation
- Modular design with reusable functions
- Professional presentation without excessive complexity
- Academic-style reporting and analysis

### Learning Objectives
- Understanding of transformer architecture applications
- Practical experience with fine-tuning pre-trained models
- Implementation of end-to-end NLP pipeline
- Evaluation and interpretation of model performance

## Limitations and Considerations

- **Dataset Size**: Uses subset for practical training time
- **Computational Resources**: Optimized for standard hardware
- **Model Complexity**: Simplified for educational purposes
- **Domain Specificity**: Focused on movie review sentiment

## Future Extensions

- Full dataset training for improved performance
- Multi-class sentiment analysis (positive/negative/neutral)
- Cross-domain sentiment analysis evaluation
- Advanced transformer architectures (RoBERTa, DistilBERT)
- Real-time sentiment analysis deployment

## Technical Notes

- Compatible with both CPU and GPU execution
- Memory-efficient implementation with appropriate batch sizes
- Error handling for common issues (missing dependencies, data loading)
- Progress tracking for long-running training processes

---

## License

This project is for educational purposes as part of AAI-520 coursework at the University of San Diego.

*Last Updated: September 2025* 