# ecgClustering
Separate the QRS signal of Fetal and Maternal!


### the first prototype
. The dataset can be founded at https://physionet.org/content/adfecgdb/1.0.0/
. I apply kmeans clustering algorithms on the first women ECG signal
. Lowpass and highpass filtering applied in this version.
. window size tunning applied in this version.
. this version is on the Jupyter Notebook.

### added post processing for false negatives
False Negatives occure when QRS of fetal have overlap with MAternal QRS, so we lost that fetal R peak, in the fetal cluster list, if the distance between two consecutive samples was larger than usual, it means that we lost a sample between those samples, so we calculate the lost sample. 