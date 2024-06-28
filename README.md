# Precision-Agriculture-through-ARVI-Based-Segmentation-of-Agave-Weber-using-UAV-Multispectral-Imaging
Segmentation of Agave plants using ARVI with UAV multispectral images

Related paper:

Data can be downloaded in: 
The data of the images are tif files with the multispectral data of the image
The image size is 224x224, it means the shape of the corresponding file is (9, 224, 224)

Blue -------> Channel 0
Green ------> Channel 1
Red --------> Channel 2
Red edge ---> Channel 3
NIR --------> Channel 4
ARVI -------> Channel 5
ARVI2 ------> Channel 6 (ARVI was computed with shadow improvement of the BGR channels)
Target -----> Channel 7 
Background -> Channel 8 (it contains the corresponding tile of the the orthomosaic map shape)

The folder contains the Jupyter notebook of the experiments described in the paper. The shadow improvement described exhibits an important increase in the evaluated metrics, making it a useful technique that does not require additional computational resources such as GPUs. It also shows a consistent improvement over each image, which means a more robust method to segment the images to make a later process for precision agriculture.

![instanceComparison](https://github.com/DiegoVillatoro/Precision-Agriculture-through-ARVI-Based-Segmentation-of-Agave-Weber-using-UAV-Multispectral-Imaging/assets/45828192/53ca56b9-9bff-4048-b9dd-3d4047032320)

The Unet model tested was trained using the provided jupyter notebook Unet.ipynb
