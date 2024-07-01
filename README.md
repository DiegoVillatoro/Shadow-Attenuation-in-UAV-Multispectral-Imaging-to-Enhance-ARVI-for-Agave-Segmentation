# Precision-Agriculture-through-ARVI-Based-Segmentation-of-Agave-Weber-using-UAV-Multispectral-Imaging
Segmentation of Agave plants using ARVI with UAV multispectral images

Related paper:

<p>Data can be downloaded in: https://figshare.com/s/bf74681957a2e3c20ba1</p>
The data of the images are tif files with the multispectral data of the image
The image size is 224x224, it means the shape of the corresponding file is (9, 224, 224)

<ul>
<li>Blue  -------> Channel 0</li>
<li>Green  ------> Channel 1</li>
<li>Red  --------> Channel 2</li>
<li>Red edge  ---> Channel 3</li>
<li>NIR  --------> Channel 4</li>
<li>ARVI  -------> Channel 5</li>
<li>ARVI2  ------> Channel 6 (ARVI was computed with shadow improvement of the BGR channels)</li>
<li>Target  -----> Channel 7 </li>
<li>Background  -> Channel 8 (it contains the corresponding tile of the the orthomosaic map shape)</li>
</ul>

The folder contains the Jupyter notebook of the experiments described in the paper. The shadow improvement described exhibits an important increase in the evaluated metrics, making it a useful technique that does not require additional computational resources such as GPUs. It also shows a consistent improvement over each image, which means a more robust method to segment the images to make a later process for precision agriculture.

![instanceComparison](https://github.com/DiegoVillatoro/Precision-Agriculture-through-ARVI-Based-Segmentation-of-Agave-Weber-using-UAV-Multispectral-Imaging/assets/45828192/53ca56b9-9bff-4048-b9dd-3d4047032320)

The Unet model tested was trained using the provided jupyter notebook Unet.ipynb
