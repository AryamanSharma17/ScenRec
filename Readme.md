## Les Furnitures 
[Aryaman Sharma](https://github.com/AryamanSharma17) and [Shani Israelov](https://github.com/shani1610)

![Picture1](https://github.com/AryamanSharma17/ScenRec/assets/56839113/e611fdc5-b539-40f9-b73e-09ab3187a51d)

This repository contains "Les Furnitures", a 3D Room Representation using a single image: A master project done for the "Complex Computer Rendering Methods in Real Time" course at Jean Monnet University. By using GroundingDINO and SegmentAnything we detect the furniture and by using ZoeDepth we calculate the relative depth. 
Finally, we introduce a visualization in a browser or VR using Three.js.

## Usage
Clone the repository by running the following in terminal:
``
git clone https://github.com/AryamanSharma17/ScenRec.git
``

run the notebook *Grounded-SAM-Zoe.ipynb*

The test images are stored [here](https://github.com/AryamanSharma17/ScenRec/tree/master/Resource/Test_images)

To test your own image, add the path to the [notebook](https://github.com/AryamanSharma17/ScenRec/blob/master/Grounded-SAM-Zoe.ipynb) cell 13
>test_image = dirmain + ...

## Resources

Material related to our project is available via the following links:

- Inspiration: https://machinelearning.apple.com/research/roomplan
- GroundingDINO Github repo: https://github.com/IDEA-Research/GroundingDINO
- SAM Github repo: https://github.com/facebookresearch/segment-anything
- ZoeDepth Github repo: https://github.com/isl-org/ZoeDepth

## Future work 
* Orientation Detection from a single image 
* More furniture categories
* More complex scenarios 
* Realistic representation 
* GUI for changes
* Change from notebook to prompt 
* Add warnings for cases nothing has been detected

## Acknowledgements

We thank the authors of GroundingDINO, SAM, and ZoeDepth, we used their GitHub and hugging face demos and notebooks. 
We thank our professor Philippe Colantoni for the advice. 

## Additional Notes about the process

#### 08.06.2023

Leres model added

Visualization Possible

Erosion Disregarded

File formatting done

#### 05.06.2023
`Leres`
1. For each mask, do separate erosion
2. Erosion can be: 3,3 kernel on small images based on a simple mask
3. For each eroded mask, do a depth center calculation
~~4. Move all setup files to the top~~
~~5. Move all test files to the bottom~~
6. If possible, move all models, etc to another file

 
`ZOE`
~~1. Do the same as Leres~~


`GENERAL`
1. Add Stereo-from-Mono by NianticLabs
2. Add MiDaS
3. git= google-research-datasets/Objectron

