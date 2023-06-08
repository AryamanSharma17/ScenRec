## Les Furnitures 
[Aryaman Sharma](https://github.com/AryamanSharma17) and [Shani Israelov](https://github.com/shani1610)

![Teaser image]()

This repository contains "Les Furnitures", 3D Room Representation using a single image, a master project done in "Complex Computer Rendering Methods in Real Time" class in Jean Monnet University. By using GroundingDINO and SegmentAnything we detect the furnitures and by using ZoeDepth we calculate the relative depth and orientation. 
Finally, we introduce a visualization in browser or VR using Three.js.

## Usage
Clone the repository by running:
``
git clone https://github.com/AryamanSharma17/ScenRec.git
``

run the notebook *Grounded-SAM-Zoe.ipynb*

## Resources

Material related to our project is available via the following links:

- Inspiration : https://machinelearning.apple.com/research/roomplan
- GroundingDINO Github repo: https://github.com/IDEA-Research/GroundingDINO
- SAM Github repo: https://github.com/facebookresearch/segment-anything
- ZoeDepth Github repo: https://github.com/isl-org/ZoeDepth

## Examples: # DO TO:

we provided some examples you can open in browser.
| Path | Description
| :--- | :----------
| [StyleGAN](https://drive.google.com/open?id=1uka3a1noXHAydRPRbknqwKVGODvnmUBX) | Main folder.
| &boxvr;&nbsp; [stylegan-paper.pdf](https://drive.google.com/open?id=1v-HkF3Ehrpon7wVIx4r5DLcko_U_V6Lt) | High-quality version of the paper PDF.
| &boxvr;&nbsp; [stylegan-video.mp4](https://drive.google.com/open?id=1uzwkZHQX_9pYg1i0d1Nbe3D9xPO8-qBf) | High-quality version of the result video.
| &boxvr;&nbsp; [images](https://drive.google.com/open?id=1-l46akONUWF6LCpDoeq63H53rD7MeiTd) | Example images produced using our generator.
| &boxv;&nbsp; &boxvr;&nbsp; [representative-images](https://drive.google.com/open?id=1ToY5P4Vvf5_c3TyUizQ8fckFFoFtBvD8) | High-quality images to be used in articles, blog

## Acknowledgements

We thank the authors of GroundingDINO, SAM and ZoeDepth, we used their github and hugging face demos and notebooks. 
We thank our professor Phillip Colantoni for the advices. 

## Additional Notes about the process

#### 05.06.2023
`leres`
1. For each mask, do separate erosion
2. Erosion can be: 3,3 kernel on small images based on simple mask
3. For each eroded mask, do depth center calculation
4. Move all setup files to the top
5. Move all test files to the bottom
6. If possible, move all model etc to another file

 
`ZOE`
1. Do same as leres


`GENERAL`
1. Add Stereo-from-Mono by NianticLabs
2. Add MiDaS
3. git= google-research-datasets/Objectron
