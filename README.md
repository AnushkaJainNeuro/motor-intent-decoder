# motor-intent-decoder
An EEG-based brain-computer interface decoder for motor imagery classification.

Built from scratch over summer 2026 as my first serious neurotech project. 
The goal is to understand the full pipeline behind systems like Neuralink — 
from raw electrode signals to decoded movement intent.

## the problem
A paralyzed person thinks "move my hand." Neurons fire. The signal travels 
through skull and scalp and gets recorded as EEG. Most of what's recorded 
is noise. The real question: can we reliably decode left vs right hand 
movement intention from that noisy signal?

## the pipeline
1. Load real EEG data (BCI Competition IV Dataset 2a)
2. Filter and clean the signal
3. Epoch into labeled trials (left hand / right hand / rest)
4. Extract CSP features (common spatial patterns)
5. Train and evaluate classifiers (LDA and EEGNet)
6. Visualize everything honestly — including what doesn't work

## tools
Python · MNE-Python · scikit-learn · PyTorch · Streamlit

## status
In active development — summer 2026
