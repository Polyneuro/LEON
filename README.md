<img src="images/LEON-Logo.png" align="left" width="80" height="80" style="margin-right: 15px;">

# LEON (Life Emulating Orchestrated Net)

This repository is a work in progress. Code is being cleaned and migrated here according to the structure below.
<br clear="left"/>

## Planned Directory Structure
```
| `/core`
|     /engine.py     # The Canonical LEON 0.32 (Scale-Agnostic)
|     /ensemble.py   # The 7-Model "Council of Experts" logic  
| `/adapters`
|     /vision.py     # Image reshaping (MNIST, CIFAR, MRI slices)
|     /signal.py     # 1 tp 2D mapping of Time series (EEG, ECG)
|     /genomics.py   # 1 to 2D mapping of genomic data
| `/experiments`     # Project experiemnts
| `/data`            # Saved Results
| 
```

## engine.py
```
LEON 0.32 has the following structure:
        1) Context Preserving Tree
        2) Dirichlet Multinomial inspired Lateral Inhibitio
        3) XOR-XNOR recursion
All three subsections involve creation of a binary out put and the final output is a concatenation binary data. This is the input to a 7 model council of experts (ML models that has a much smaller feature space to go through and output a probability vector).

```
