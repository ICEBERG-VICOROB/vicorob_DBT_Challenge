# VICOROB DBT Challenge participation

Participation on the DBT Challenge http://spie-aapm-nci-dair.westus2.cloudapp.azure.com/competitions/4 from the VICOROB research group (University of Girona, Spain). 

Contact: Robert Marti, robert.marti@udg.edu


Using functions from duke-dbt-data 

https://github.com/MaciejMazurowski/duke-dbt-data


## Vicorob additions

- pre_process_rm.ipynb

Pre-processing of DBT images to generate 2D slices and bounding boxes to be trained in detectron

- DBT_detectron.ipynb

Implementation of detectron training with the OMIDB and DBT dataset

- inference_DBT.ipynb

Inference of new images (validation provided in the web page)

# Used from dubke-dbt-data

## read dicom image

`dcmread_image.ipynb` notebook shows how to read image data from a DICOM file in the coordinate system that maches the ground truth bounding boxes.

## draw bounding box

`draw_box.ipynb` notebook shows how to draw a bounding box on the image.

## helper functions

To use helper functions from the notebooks, simply copy the `duke_dbt_data.py` file to your project.
