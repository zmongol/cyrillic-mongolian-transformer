# Cyrillic-Mongolian Transformer

A bidirectional Transformer-based character-level neural model for seamless conversion between Cyrillic and Traditional Mongolian scripts.

## Overview

This repository contains a state-of-the-art deep learning solution for Cyrillic ↔ Traditional Mongolian script transformation. Unlike traditional rule-based converters or simple character mappings, this project leverages a full sequence-to-sequence Transformer architecture trained on aligned parallel text, enabling:

- **Robust contextual handling**: Correctly manages variant glyphs based on context
- **Noise tolerance**: Handles real-world imperfections in text data
- **Bidirectional support**: Independent models for both transformation directions
- **Production-ready**: Extensible architecture suitable for OCR, IME, and NLP pipelines

## Model Architecture

The system uses a Transformer-based sequence-to-sequence model with:
- Character-level tokenization
- Separate vocabularies for Cyrillic and Traditional Mongolian
- Independent training for each direction to optimize accuracy

### Supported Directions

1. **Cyrillic → Traditional Mongolian** (`cyr2mng`)
2. **Traditional Mongolian → Cyrillic** (`mng2cyr`)

## Files

- `cyr2mng_Gemini3.ipynb` - Jupyter notebook for Cyrillic to Mongolian conversion training and inference
- `cyr2mng_best_model_Gemini3.pth` - Trained model weights for Cyrillic → Traditional Mongolian
- `mng2cyr__Gemini.ipynb` - Jupyter notebook for Mongolian to Cyrillic conversion training and inference
- `mng2cyr_best_model.pth` - Trained model weights for Traditional Mongolian → Cyrillic
- `20260101_K-M_YiTailvarTolin_Tolgai uguud.txt` - Reference text data

## Usage

### Requirements

- Python 3.8+
- PyTorch
- Jupyter Notebook
- Standard NLP libraries (numpy, pandas, etc.)

### Running the Models

1. **Open the desired notebook**:
   ```bash
   jupyter notebook cyr2mng_Gemini3.ipynb
   # or
   jupyter notebook mng2cyr__Gemini.ipynb
   ```

2. **Load the pre-trained model** and use it for inference on your text

3. **Customize and retrain** if needed for specific datasets

## Project Details

This project addresses the critical need for accurate script conversion in Mongolian NLP and digital humanities applications. The Transformer architecture provides superior performance compared to traditional approaches by:

- Learning complex character transformation rules from data
- Handling ambiguous mappings through context awareness
- Supporting various text encodings and variants

## About

This project is developed to advance Mongolian script digitization and NLP, focusing on:
- Writing systems & Unicode architecture
- Mongolian script transformation
- AI/NLP for low-resource languages
- Integration with broader linguistic tools

## License

[Add appropriate license information here]

## Citation

If you use this model in your research, please cite:

```bibtex
@project{cyr2mng_transformer,
  title={Cyrillic-Mongolian Transformer},
  year={2026},
  url={https://github.com/zmongol/cyrillic-mongolian-transformer}
}
```

## Contact & Contributions

For questions, issues, or contributions, please open an issue on the GitHub repository.

---

**Note**: This model works best with properly formatted input text. Pre-processing of text (normalization, encoding verification) may improve results for specific use cases.
