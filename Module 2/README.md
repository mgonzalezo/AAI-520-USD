# NLP Analysis: Named Entity Recognition (NER) and Part-of-Speech (PoS) Tagging

## Climate Fever Dataset Analysis

**Author:** Marco Gonzalez  
**Course:** AAI-520-IN2  

This project performs comprehensive Natural Language Processing analysis on the Climate Fever dataset, focusing on Named Entity Recognition (NER) and Part-of-Speech (PoS) tagging to extract insights from climate-related claims.

## 🎯 Project Overview

The analysis includes:
- **Named Entity Recognition**: Identifying and classifying entities (persons, organizations, locations, dates, etc.)
- **Part-of-Speech Tagging**: Analyzing grammatical structure and word categories
- **Data Visualization**: Interactive dashboards, word clouds, and statistical charts
- **Advanced Analysis**: Entity-PoS relationships, climate-specific terminology, sentiment analysis

## 📁 Project Structure

```
archive/
├── 2-1-NLP-NER-PoS-Tagging-Marco-Gonzalez.ipynb  # Main analysis notebook
├── climate-fever.csv                              # Dataset (1,535 climate claims)
├── requirements.txt                               # Python dependencies
└── README.md                                      # This file
```

## 🚀 Setup Instructions

### 1. Prerequisites
- Python 3.8 or higher
- pip package manager

### 2. Install Dependencies

```bash
# Clone or download the project files
cd /path/to/archive

# Install Python packages
pip install -r requirements.txt

# Download spaCy English language model
python -m spacy download en_core_web_sm
```

### 3. Verify Installation

```python
# Test imports
import pandas as pd
import spacy
import nltk

# Test spaCy model
nlp = spacy.load("en_core_web_sm")
print("✅ Setup complete!")
```

## 📊 Dataset Information

- **Source**: Climate Fever dataset
- **Size**: 1,535 climate-related claims
- **Format**: CSV with claims and supporting evidence
- **Analysis Sample**: 500 claims for detailed NLP processing

## 🔧 Key Features

### Named Entity Recognition
- Identifies 15+ entity types (PERSON, ORG, GPE, DATE, CARDINAL, etc.)
- Climate-specific entity analysis
- Entity frequency and distribution analysis

### Part-of-Speech Tagging
- Comprehensive grammatical analysis
- Word category distribution
- Linguistic pattern identification

### Visualizations
- Interactive Plotly dashboards
- Word clouds for entity types
- Statistical charts and distributions
- Box plots and pie charts

### Advanced Analysis
- Entity-PoS relationship mapping
- Climate terminology identification
- Sentiment analysis by entity type
- Domain-specific insights

## 📈 Expected Results

The analysis provides:
- **Quantitative Metrics**: Entity counts, PoS distributions, statistical summaries
- **Visual Insights**: Interactive charts showing patterns and relationships
- **Linguistic Analysis**: Grammatical structure and vocabulary patterns
- **Domain Insights**: Climate-specific terminology and entity patterns

## 🏃‍♂️ Running the Analysis

1. **Start Jupyter**: 
   ```bash
   jupyter notebook
   ```

2. **Open the notebook**: 
   `2-1-NLP-NER-PoS-Tagging-Marco-Gonzalez.ipynb`

3. **Run all cells**: 
   - Execute cells sequentially
   - First-time run will download NLTK resources automatically
   - Analysis takes ~5-10 minutes for the sample dataset

## 📋 Requirements

### Core Libraries
- `pandas>=2.0.0` - Data manipulation and analysis
- `numpy>=1.24.0` - Numerical computing
- `matplotlib>=3.6.0` - Static plotting
- `seaborn>=0.12.0` - Statistical visualization

### NLP Libraries
- `nltk>=3.8.0` - Natural language toolkit
- `spacy>=3.6.0` - Advanced NLP processing
- `textblob>=0.17.0` - Sentiment analysis

### Visualization
- `wordcloud>=1.9.0` - Word cloud generation
- `plotly>=5.15.0` - Interactive visualizations

### Additional
- `networkx>=3.1.0` - Graph analysis utilities

## 🔍 Analysis Sections

1. **Setup & Data Loading**: Environment setup and dataset exploration
2. **Preprocessing**: Text cleaning and preparation
3. **NER Analysis**: Entity extraction and classification
4. **PoS Analysis**: Grammatical structure analysis
5. **Visualization**: Interactive dashboards and charts
6. **Advanced Analysis**: Relationships and domain-specific insights
7. **Summary**: Key findings and conclusions

## 🎨 Visualization Examples

- **NER Dashboard**: Entity type distributions and frequency analysis
- **PoS Dashboard**: Grammatical category analysis and word length distributions
- **Word Clouds**: Visual representation of entities and common terms
- **Statistical Charts**: Bar plots, pie charts, and box plots

## 🔬 Technical Approach

- **Multi-library Analysis**: Combines spaCy and NLTK for comprehensive results
- **Performance Optimization**: Sample-based analysis for large datasets
- **Interactive Visualization**: Plotly for dynamic data exploration
- **Error Handling**: Robust error handling for missing dependencies
- **Modular Design**: Clear separation of analysis components

## 📊 Expected Insights

- Climate claims contain diverse named entities with global geographic scope
- Rich grammatical structure indicates scientific discourse complexity
- Quantitative focus with high presence of numerical and temporal entities
- Domain-specific terminology patterns in climate communication

## 🚧 Troubleshooting

### Common Issues

1. **spaCy model not found**:
   ```bash
   python -m spacy download en_core_web_sm
   ```

2. **NLTK download errors**:
   - Check internet connection
   - Try manual download: `nltk.download('punkt')`

3. **Memory issues with large dataset**:
   - Reduce `SAMPLE_SIZE` variable in the notebook
   - Close other applications to free memory

4. **Visualization not displaying**:
   - Ensure Jupyter supports interactive widgets
   - Try: `pip install ipywidgets`

## 📞 Support

For questions or issues:
- Check the troubleshooting section above
- Review error messages for specific guidance
- Ensure all dependencies are properly installed

## 📄 License

This project is for educational purposes as part of AAI-520-IN2 coursework. 