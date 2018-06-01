# conefinder-yolo
Traffic Cone Finder using Alexey AB's Windows Yolo implementation
https://github.com/AlexeyAB/darknet


Extract dataset.rar given in Dropbox link to the data folder here.
Dataset is extracted from DukeCone's dataset and manually annotated. https://github.com/melfm/dukecone

Download the yolo-obj_3200.weights file also from Dropbox link and put to root.

Run command

```darknet.exe detector test data/obj.data yolo-obj.cfg yolo-obj_3200.weights data/img1/cone0611.jpg```

To predict cones in the cone0611.jpg image. This is the image used in the report.

To use for videos;

```darknet.exe detector demo data/obj.data yolo-obj.cfg yolo-obj_3200.weights test.mp4 -i 0 -out_filename res.avi```

This will take the test.mp4 and output res.avi with the predicted boundary boxes with yolo-obj_3200.weights file.
