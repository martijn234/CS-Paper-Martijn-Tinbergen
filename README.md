# CS-Paper-Martijn_Tinbergen
This project implements the Scalable Duplicate Detection with Pre-selection Method (SDDPM), leveraging LSH with dropout and TF-IDF-based feature selection to address the challenges of duplicate detection in e-commerce. The dataset employed for this study comprises 1624 descriptions of televisions
originating from four web shops. It can be accessed at: https://personal.eur.nl/frasincar/datasets/TVs-all-merged.zip.
The provided code is written in Python.
We start with data cleaning. For every product, the title is used to extract important model words using TF-IDF scores and obtain a binary vector representation for
each product. The binary vectors are transformed into a signature vector through the process of min-hashing. These signature vectors are used to obtain candidate duplicate pairs using LSH with a drop-out mechanism. Lastly, hierarchical complete-linkage clustering is used to obtain the final set of duplicates.
