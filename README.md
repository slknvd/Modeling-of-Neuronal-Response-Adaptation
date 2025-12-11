# Investigating Neuronal Adaptation to Repeated Natural Stimuli in the Visual Cortex

A neuroscience data analysis project exploring how mouse visual cortex neurons adapt when repeatedly exposed to natural images. We examine firing-rate changes, compare regular-spiking (RS) vs. fast-spiking (FS) neurons, and evaluate how stimulus timing influences adaptation.

## How It's Made

Tech used:
Python, NumPy, Pandas, Matplotlib, Scikit-learn, OpenCV, Jupyter Notebook, Allen Brain Observatory dataset.

This project investigates neural adaptation—the reduction in neuronal firing when a stimulus is repeated. Using large-scale electrophysiology data from mice, the project includes:

Classification of neurons into RS and FS using waveform duration and firing rate

Filtering for visually responsive neurons based on evoked vs. spontaneous activity

Adaptation metrics: delta firing rate, slope, Spearman correlation, Fano factor

PCA to combine adaptation metrics and study population activity

Temporal analysis of different image presentation schedules

Image feature extraction using OpenCV (brightness, contrast, edges, spectral slope)

The initial hypothesis was that RS neurons adapt more strongly than FS neurons. Results did not support this.

## Key Results

1. RS neurons adapt most under increasing-frequency presentations (Frame 18).

Strong drop in firing rate

Significant t-test difference

Clear early vs. late PCA separation

2. Uniform presentation schedules show minimal adaptation (Frame 0).

3. FS neurons adapted more than RS neurons in the most adaptation-prone condition.

Larger reduction in responses

More significant p-value

Must be interpreted cautiously due to small FS sample size (49 neurons)

4. Brighter images were associated with less adaptation among highly adaptive scenes
