# Unicamp-UAV Dataset

## Dataset for human detection in UAV images 

Human detection in UAV images has proven to be significant for a wide range of applications, including search and rescue operations, crowd counting for public safety, surveillance, and military operations. Emerging activities have also benefited from human detection in UAV imagery. For instance, in planning safe routes for UAVs, human detection in UAV images obtained in real-time can ensure a minimum distance between the UAV and people along the route, as defined by UAV operation regulations in some countries.

Despite significant progress in person detection with the deep learning era, it remains a challenging task. UAV imagery can be considered a special case of small or even tiny object detection - such as people in UAV images. The variable size of individuals, diverse human poses, complex backgrounds, and the large volume of data in UAV images, combined with varying lighting conditions and different heights and perspectives from which images are captured, all contribute to the complexity this task. Considering these particularities, the quality of the dataset used to train the deep learning model for object detection is crucial to achieving reliable results. Despite the availability of publicly accessible datasets, finding an appropriate dataset for a specific, large-scale application that is accurately annotated is challenging. 

To contribute to the scientific community focused on small object detection and UAV applications, we present a dataset for person detection in UAV images, named "Unicamp-UAV." This dataset was created by recording three videos at 30 FPS with a DJI Phantom 4 UAV at different locations by the Barão Geraldo Campus of Unicamp / Brazil. The videos were captured in daylight and under suitable weather conditions, aiming for different camera orientations and individuals in various poses to ensure data heterogeneity and produce a representative dataset for the area of interest. After preprocessing and data cleaning, 6,500 images were selected to compose the dataset. Among these, 6,000 images contain people (positives images), labeled using the LabelImg tool, and 500 are negative images, i.e., containing only background information. The dataset was subdivided into training, validation, and testing sets, as shown in the table below.

|Data | Sampled images| Object instances| 
|-------------|-------------|-------------| 
|Train| 4160| 35968|
|Validation| 1040| 9617|
|Test| 1300 | 12970|
|Total| 6500 | 58555|

Representative images from our dataset are presented below.

<table>
  <tr>
    <td><img src="https://github.com/SimoesDP/Unicamp-UAV-Dataset/blob/main/Repository%20figures/DJI_0083_2224.jpg" alt="Descrição 1" width="300"/></td>
    <td><img src="https://github.com/SimoesDP/Unicamp-UAV-Dataset/blob/main/Repository%20figures/DJI_0084_2062.jpg" alt="Descrição 2" width="300"/></td>
  </tr>
  <tr>
    <td><img src="https://github.com/SimoesDP/Unicamp-UAV-Dataset/blob/main/Repository%20figures/DJI_0084_6589.jpg" alt="Descrição 3" width="300"/></td>
    <td><img src="https://github.com/SimoesDP/Unicamp-UAV-Dataset/blob/main/Repository%20figures/DJI_0084_7384.jpg" alt="Descrição 4" width="300"/></td>
  </tr>
</table>


## Dataset Info
- Bounding box annotations are available in text format for all the train, validation, and test sets separately;
- Some of the test images and labels are provided in this repo for simple inference purposes and can be found in the [Test Images - Sample]( https://github.com/SimoesDP/Unicamp-UAV-Dataset/tree/main/Test%20Images%20-%20Sample) and [Test Labels - Sample]( https://github.com/SimoesDP/Unicamp-UAV-Dataset/tree/main/Test%20Labels%20-%20Sample) folders, respectively;
- All the images in the dataset are color images (RGB) with a resolution of 3840 x 2160 pixels.

## Access to data

- This dataset is intended for academic research only and should not be used for commercial applications;
- To access the dataset, visit [Unicamp-UAV](https://drive.google.com/drive/folders/1ZpdnmakLtd6gXynRRjebpSZ1rD3TfehJ?usp=sharing);
- If you use our dataset in your work, please cite us:

_SIMÕES, D. P.; OLIVEIRA, H. C.; MARSICO, S.; SOUZA, J. R.; BARBOSA, L. A. Advancements in human detection using UAV imagery: the Unicamp-UAV dataset and a comparison of recent YOLO models. ISPRS Journal of Photogrammetry and Remote Sensing. 2025. Submitted for publication._
