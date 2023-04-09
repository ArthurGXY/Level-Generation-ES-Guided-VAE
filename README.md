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
7. Generated levels are saved under "./GPU/generated_levels" if running on GPU. If it is run on CPU, the folder is "./CPU/generated_levels"

### Remarks:
1. We separate "GPU" and "CPU" since there are difference between the two modes that cannot be merged easily.
2. The "TensorFlow(abandoned)" folder contains our attempt of building the VAE from scratch. However, it suffers from overfitting issues and we do not have enough time to figure that out.
3. The code we use for VAE are in "./CPU/utility" and "./GPU/utility", which come from (the source code of)[https://github.com/yoshinobc/Level-Generation-for-Angry-Birds-with-Sequential-VAE-and-Latent-Variable-Evolution/tree/main/generator].

### Reference:
1. Takumi Tanabe, Kazuto Fukuchi, Jun Sakuma, and Youhei Akimoto. 2021. Level Generation for Angry Birds with Sequential VAE and Latent Variable Evolution. In Proceedings of the Genetic and Evolutionary Computation Conference (Lille, France) (GECCO ’21). Association for Computing Machinery, New York, NY, USA, 1052–1060. <https://doi.org/10.1145/3449639.34592>
