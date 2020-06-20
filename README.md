# Youtube-Trending-ML

This repository contains the machine learning part of the YouTube-trending analysis.
To see how the data is being collected please have a look at [this repository](https://github.com/MartenPrecht/Youtube-Trending-Downloader).
The amount of required filtering is calculated based on the thumbnail and the title of the video.
Both parts are evaluated separately and will be combined into a single score in the extension.

## Thumbnail based evaluation
In this part we train an NN to distinguish the thumbnails of trending videos from videos sampled from my subscription feed.
To do this we retrain a MobileNet that was trained on ImageNet.
The training takes place in the **`trainig.ipynb`**.
In the **`tf_lite_test.ipynb`** we can see an example prediction implementation together with the prediction of a few thumbnails (that were part of the training process).

## Title based prediction
This section will contain information about the title based prediction once it is implemented.
It is planned to be based on an sentiment analysis architecture.
