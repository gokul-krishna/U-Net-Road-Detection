# U-Net Road Detection
Initially I planned on training U-Net on the [Massachusetts Roads Dataset](https://www.cs.toronto.edu/~vmnih/data/). This  [notebook](get_MA_road_data.ipynb) contains the code to download and collate the data, but some of the training images seems to be corrupted, like this [for example](http://www.cs.toronto.edu/~vmnih/data/mass_roads/train/sat/11278645_15.tiff).

So, I decided to create my own dataset, using the satellite and road/terrain layers of Google Maps. In [this notebook](get_GMaps_data.ipynb) you can find all the code required to create your own dataset using Google Maps APIs and other the transformation required to prepare the images/masks for training.

This [notebook](U-Net_FastAI.ipynb) contains the implementation using fastAI library, and a pure [PyTorch Implementation](U-Net_PyTorch.ipynb) is currently work in progress.

## Results
![Results](/images/result.png)
