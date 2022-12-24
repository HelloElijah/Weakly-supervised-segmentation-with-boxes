# Yolo_v1_from_scratch

## Download dataset(5GB) from Kaggle into Google Colab with the following command
```bash
!pip install -q kaggle
from google.colab import files
files.upload()
```
Upload the kaggle.json file, can follow the tutorial if necessary (https://www.kaggle.com/general/74235)
```bash
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

```bash
!kaggle datasets download -d aladdinpersson/pascal-voc-dataset-used-in-yolov3-video
```

```bash
!unzip pascal-voc-dataset-used-in-yolov3-video.zip
```

## Reference
1. Most idea from Yolo's paper:
Redmon, J., Divvala, S., Girshick, R., & Farhadi, A. (2016). You only look once: Unified, real-time object detection. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 779-788).

2. The code from external library:
https://github.com/aladdinpersson/Machine-Learning-Collection/blob/master/ML/Pytorch/object_detection/YOLO/utils.py

3. Full dataset can be retrieve from https://www.kaggle.com/datasets/aladdinpersson/pascal-voc-dataset-used-in-yolov3-video. The code for uploading the dataset from kaggle to colab can be found in the appendix.
4. Get a better understanding about Yolo after watch the video:
https://www.youtube.com/watch?v=n9_XyCGr-MI&list=PLhhyoLH6Ijfw0TpCTVTNk42NN08H6UvNq&index=6
