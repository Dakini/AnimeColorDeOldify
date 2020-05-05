
# Anime/Sketch/Manga Coloriser trained with DeOldify
![](https://i.imgur.com/UnAsqFr.jpg)

This repo is based on the work of Jason Antic, the creator of DeOldify. I have used his code base, to bring you this repository that allows you to colorise anime/manga sketches.

**Quick Start**: The easiest way to colorize images using This model trained via DeOldify (for free!) is via one of the colabs below!

----------------------------

Image  [<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/Dakini/AnimeColorDeOldify/blob/master/ImageColorizerColab.ipynb) 

GrayScale Images [<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/Dakini/AnimeColorDeOldify/blob/master/ImageColorizerColabGrayScale.ipynb)

Digital Sketches [<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/Dakini/AnimeColorDeOldify/blob/master/ImageColorizerColabSketch.ipynb)

Sketches to Shading (tempremental) [<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/Dakini/AnimeColorDeOldify/blob/master/ImageColorizerColabSketch2Gray.ipynb)


The easiest way to learn how to use the Colabs, are the same those used in the DeOldify repository, which has kinldy been provided by  in video tutorial form by Old Ireland in Colour's John Breslin. Click video image below to watch.

[![](http://img.youtube.com/vi/VaEl0faDw38/0.jpg)](http://www.youtube.com/watch?v=VaEl0faDw38)

Get more updates here [Twitter <img src="resource_images/Twitter_Social_Icon_Rounded_Square_Color.svg" width="16">](https://twitter.com/CpnTaters).

## More to be filled out shortly

## About this Repository
The goal for project this was to recolorise manga into color. Its been one of the main things I have wanted to do with deep learning and after experimenting with DeOldify, I wanted to try it with the danbooru2019 dataset.

Here are some pictures from this model. 

## Example Grayscale Images
[![](https://i.imgur.com/6ILHXKv.png)

[![](https://i.imgur.com/jWal2Yy.png)

[![](https://i.imgur.com/bIjzL4Y.png)

[![](https://i.imgur.com/hkEY8xw.png)

[![](https://i.imgur.com/u7VnO8G.png)

[![](https://i.imgur.com/SxkCbSV.png)

## Example Sketch images
[![](https://i.imgur.com/Pv55JR0.png)

[![](https://i.imgur.com/txFXt3h.png)

[![](https://i.imgur.com/0h6npGK.jpg)

[![](https://i.imgur.com/bPApVZG.jpg)

[![](https://i.imgur.com/ht5Tl5M.jpg)

## Manga Colorisation

[![](https://pbs.twimg.com/media/EXPlda8X0AEdtUx?format=jpg&name=4096x4096)

[![](https://pbs.twimg.com/media/EW3NDhMX0AEhl6y?format=jpg&name=medium)

[![](https://pbs.twimg.com/media/EW3NEQBWsAAsouA?format=jpg&name=small)

[![](https://pbs.twimg.com/media/EXQrJnBXsAEEwbz?format=jpg&name=medium)

[![](https://pbs.twimg.com/media/EXQrLAbWsAMBpAb?format=png&name=900x900)

[![](https://pbs.twimg.com/media/EW3NBweWAAIjwA_?format=jpg&name=medium)

## Why four models

This repository contains four models, All trained using the same code but different datasets. They are all based on the artistic training code that is provided by DeOldify [DeOldify]. They are the Image coloriser,Grayscale2Color, Sketch2Color, and Sketch2Gray.

As described in the DeOldify repo. The Artistic model acheives the highest quality in image coloriosation, in terms of interesting details and vibrance, which is needed for any dataset based on art especially Danbooru. However, the model can be particular on getting the best results, which can be adjusted using the render setting. The best setting is currently 12, but a higher render_factor is needed for rendering manga. 

# Getting Started

The easiest way to get started is using the google colabs, avaialble here. [<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/Dakini/AnimeColorDeOldify/blob/master/ImageColorizerColab.ipynb) 

## Installing this repo

This should be an easy install if you have conda installed. 

```
git clone https://github.com/Dakini/AnimeColorDeOldify
cd AnimeColorDeOldify
pip install -r requirements.txt
jupyter notebook
```

My training code, is not avaiable, as its a bit of a mess at the moment, with various hacks in place. 
However, I used the same training code from the Artistic jupyter notebook avaiable on the [DeOldify repository](https://github.com/jantic/DeOldify)

I used the danbooru dataset, which you can find more information [here](https://www.gwern.net/Danbooru2019). The dataset is a total of ~3 TB, with over 3 millions images. 

To start right away on your own machine with your own images or videos without training the models yourself, you'll need to download the pretrained models.They can be found here 

- [Image](https://www.dropbox.com/s/0m1rwdk7je1r39j/MQT9QHUfXxKpQ9b2CPda89htDBzFtmHD9r2YZsHp.pth?dl=0)
- [GrayScale](https://www.dropbox.com/s/ojrwwsre1gt6sfx/UDLVQJgsv5RwrTkVWAhS9LrdGDFzdbuN2SFxCFsZ.pth?dl=0 )
- [Sketch](https://www.dropbox.com/s/lykykhvpy9byb7u/JG5yF2bRBdpEJweytyvBSz3Qu6jcg8cfZ5kcFYGY.pth?dl=0)
- [Sketch2Gray](https://www.dropbox.com/s/6me8m9e7nfmlid6/tDEFrpvevtu6WGRKf2uV5cFtsFAEhuA5kmN7FpgZ.pth?dl=0)

The colorization inference notebooks should be able to guide you from here. 

## License

All code in this repository is under the MIT license as specified by the LICENSE file.

The model weights listed in this readme under the "Pretrained Weights" section are trained by ourselves and are released under the MIT license.
