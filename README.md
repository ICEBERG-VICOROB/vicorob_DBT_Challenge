# VICOROB DBT Challenge participation

Based on duke-dbt-data 

https://github.com/MaciejMazurowski/duke-dbt-data


## Vicorob additions

- pre_process_rm.ipynb

Pre-processing of DBT images to generate 2D slices and bounding boxes to be trained in detectron

- DBT_detectron.ipynb

Implementation of detectron training with the DBT dataset

- inference_DBT_localEval.ipynb
- inference_DBT.ipynb

Inference of new images (validation provided in the web page or own dataset)



## old stuff from Duke...


## docker

Build docker image:

```
docker build -t duke-dbt .
```

Run container bash:

```
docker run --rm -it \
  -v `pwd`:/duke-dbt \
  -v /path/to/data:/data \
  -p 8889:8889 \
  duke-dbt bash
```

Replace `/path/to/data` with a path to the downloaded data folder.

## jupyter notebook

Serve jupyter notebook from the container:

```
jupyter notebook --allow-root --ip=0.0.0.0 --port=8889
```

## read dicom image

`dcmread_image.ipynb` notebook shows how to read image data from a DICOM file in the coordinate system that maches the ground truth bounding boxes.

## draw bounding box

`draw_box.ipynb` notebook shows how to draw a bounding box on the image.

## helper functions

To use helper functions from the notebooks, simply copy the `duke_dbt_data.py` file to your project.
