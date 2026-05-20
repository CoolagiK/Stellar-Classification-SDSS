# Stellar Classification using SDSS Photometric Data
Independent astrophysics and machine learning project investigating whether broadband photometry alone can recover stellar spectral classifications.

## Overview
This study uses photometric data from the Sloan Digital Sky Survey (SDSS) to classify stars along the Harvard spectral sequence (O, B, A, F, G, K, M) using supervised machine learning.
A Random Forest classifier was trained using:
- dereddened SDSS magnitudes:
  - u
  - g
  - r
  - i
  - z
- derived color index:
  - (g-r)
    
## Results
- Test Accuracy: **88.43%**
- Cross-Validated Accuracy: **89.2 ± 1.2%**
The model performed strongly for hot O/B stars while intermediate F/G/K stars exhibited expected photometric degeneracy.

## Dataset
Data was queried directly from the SDSS SpecPhoto catalog using `astroquery`.

## Tools Used
- Python
- Google Colab
- astroquery
- scikit-learn
- pandas
- matplotlib
- NumPy
  
## Files
- `stellar_classification.ipynb` → full notebook
- `Stellar_Classification_SDSS.pdf` → research paper

## Acknowledgement
AI assistance was used for portions of the Python implementation. All scientific interpretation, methodology selection, analysis, and writing were completed independently.
