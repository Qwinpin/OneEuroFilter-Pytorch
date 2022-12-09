Modification of the OneEuro filter algorithm from the repository: https://github.com/jaantollander/OneEuroFilter to handle pytorch data presented in batches of different sizes.

The input dimensionality of the data should be: (N, L, D)
- N size of the batch
- L the length of the sequence
- D dimension of the features

## Example
```
import torch
import matplotlib.pyplot as plt
from filter import filter_signal

sample = torch.randn((5, 100, 147))
sample_filtered = filter_signal(sample)

# plot one line from whole batch for example
plt.plot(sample[0, :, 0], label='origin')
plt.plot(sample_filtered[0, :, 0], label='filtered')
```
