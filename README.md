It's z-mahmud22's Mask-RCNN_TF2.14.0, but tweaked to fit the algae data.

Specifications used:
Python 3.10.12
Tensorflow 2.14.0

Create a new folder called "logs" in the parent folder

Recommended to train a new model starting from pre-trained COCO weights on anaconda:
```
python algae.py train --dataset=<where you put the dataset> --weights=coco
```

Use `get_csv_of_images.ipynb` to check model and get the csv file of "IDs", boundaries, and center point.

Apply coloring effect on an image and get csv
```
python3 algae.py splash --weights=<where your preferred weights are> --image=<file name or URL>
```

`algae.py` uses 1 epoch with 100 steps per epoch (Change this for better accuracy)



