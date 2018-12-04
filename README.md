# U-Net Road Detection
Initially I thought of training U-Net on this [Massachusetts Roads Dataset](https://www.cs.toronto.edu/~vmnih/data/). I created this [notebook](get_MA_road_data.ipynb) to download and collate the data, but the training images seem to be corrupted, like this [for example](http://www.cs.toronto.edu/~vmnih/data/mass_roads/train/sat/11278645_15.tiff).

So I thought it would be fun create our won dataset, using Google Maps layers. In [this notebook](get_GMaps_data.ipynb) you can find all the code required to create your own dataset using Google Maps APIs and other transformation on masks required in order to prepare it for training.

This [notebook](U-Net_FastAI.ipynb) contains the implementation using fastAI library, and a pure PyTorch Implementation in work in progress.

## Results
![Results](https://raw.githubusercontent.com/miragegokul/U-Net-Road_Detection/blob/master/images/result.png)
