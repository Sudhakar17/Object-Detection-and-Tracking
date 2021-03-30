# Object-Detection-and-Tracking

I use this repository to understand the Object detection and tracking workflow using YOLOV3-DeepSORT(References are mentioned below).

### Downloading official pretrained weights

```
# yolov3
wget https://pjreddie.com/media/files/yolov3.weights -O weights/yolov3.weights

# yolov3-tiny
wget https://pjreddie.com/media/files/yolov3-tiny.weights -O weights/yolov3-tiny.weights
```

### To convert the weights

```
#set the flag for tiny model
python convert.py 
```


### To Run the Object Tracker
```
python object_tracker.py --video ./data/video/test.mp4 --output ./data/video/results.avi
```


References:

1. [DeepSORT](https://github.com/nwojke/deep_sort)
2. [YOLOv3-tf](https://github.com/zzh8829/yolov3-tf2)
3. [Kalman Filter](https://www.bzarg.com/p/how-a-kalman-filter-works-in-pictures/)
