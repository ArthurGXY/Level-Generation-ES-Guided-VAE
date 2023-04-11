## Angry Birds (Science Birds) Level Generation by Evolutionary Strategy Guided Variational Autoencoder

### Play game:

1. Download the folder "build-windows". If you are using other OS, you can fetch the [Science Birds](https://github.com/lucasnfe/science-birds) repository and build it with Unity.
2. Run "Science_Birds.exe", or the binary executable you compiled.
3. Levels should be placed in folder "./build-windows/ScienceBirds_Data/StreamingAssets/Levels".

### Run EA:

1. Download the folder "GPU".
2. Upload that onto Google Colab.
3. Open "Experiment.ipynb".
4. Connect Colab to GPU.
5. Configure the variable `notebook_path` to the path of the notebook.
6. (Select a custom fitness).
7. Run all code blocks.
8. Generated levels are saved under "./GPU/generated_levels".

### Remarks:
1. We separate "GPU" and "CPU" since there are difference between the two modes that cannot be merged easily.
2. The "TensorFlow(abandoned)" folder contains our attempt of building the VAE from scratch. However, it suffers from overfitting issues and we do not have enough time to figure that out.
3. The code we use for VAE are in "saved_models" and "utility" folder, under "./CPU" and "./GPU", which are extracted and modified from [the source code of the paper we reviewed](https://github.com/yoshinobc/Level-Generation-for-Angry-Birds-with-Sequential-VAE-and-Latent-Variable-Evolution/tree/main/generator). 
4. The code to build the game environment come from [Science Birds](https://github.com/lucasnfe/science-birds).
### Reference:
1. Takumi Tanabe, Kazuto Fukuchi, Jun Sakuma, and Youhei Akimoto. 2021. Level Generation for Angry Birds with Sequential VAE and Latent Variable Evolution. In Proceedings of the Genetic and Evolutionary Computation Conference (Lille, France) (GECCO ’21). Association for Computing Machinery, New York, NY, USA, 1052–1060. <https://doi.org/10.1145/3449639.34592>
