# conefinder-yolo
Traffic Cone Finder using Alexey AB's Windows Yolo implementation


Extract dataset.rar given in Dropbox link to the data folder here.

Download the yolo-obj_3200.weights file also from Dropbox link and put to root.

Run command

```darknet.exe detector test data/obj.data yolo-obj.cfg yolo-obj_3200.weights data/img1/cone0611.jpg```

To predict cones in the cone0611.jpg image. This is the image used in the report.
