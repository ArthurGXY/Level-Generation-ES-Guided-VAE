## Angry Birds (Science Birds) Level Generation by Evolutionary Strategy Guided Variational Autoencoder

### Play game:

1. Download the folder "build-windows".
2. Run "Science_Birds.exe".
3. Levels are saved under folder "./build-windows/ScienceBirds_Data/StreamingAssets/Levels".

### Run EA:

1. If your Google Colab can run GPU, download the folder "GPU". Otherwise, download the folder "CPU".
2. Upload that onto Google Colab.
3. Open "Experiment.ipynb".
4. Configure the filepath of variable `notebook_path`.
5. (Select a custom fitness).
6. Run all code blocks.
7. Generated levels are saved under "./GPU/generated_levels".

### Remarks:
1. We separate "GPU" and "CPU" since there are difference between the two modes that cannot be merged easily.
