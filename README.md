Modification of the OneEuro filter algorithm from the repository: https://github.com/jaantollander/OneEuroFilter to handle pytorch data presented in batches of different sizes.

The input dimensionality of the data should be: (N, L, D)
- N size of the batch
- L the length of the sequence
- D dimension of the features
