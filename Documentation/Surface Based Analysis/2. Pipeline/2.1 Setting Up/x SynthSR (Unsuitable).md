[Documentation](https://github.com/BBillot/SynthSR)
[Iglesias et al. (2021)](https://www.sciencedirect.com/science/article/pii/S1053811921004833)
[Iglesias et al. (2023)](https://www.science.org/doi/10.1126/sciadv.add3607)

# SynthSR
A convolutional neural network that turns a clinical MRI scan (or even CT scan!) of any orientation, resolution and contrast into  $1mm^3$  isotropic MP-RAGE, **while inpainting lesions (which enables easier segmentation, registration, etc)**.

**SynthSR** aims to essentially get high resolution, anisotropic, and large spacing images to conform to an isotropic $1mm^3$ resolution that is required for most preprocessing. 

Our dataset is obviously continuous but suffer from the same two issues. Although it was a long shot I tried to apply SynthSR to our dataset. Surprisingly the contrast was quite good, though unsurprisingly the resolution was horrible - much worse than freesurfer. 

## Docker
If anyone is interested in using this, I've made a docker image of the env required to run SynthSR - which should save a bit of headache as the requirements are quite dated, not backwards compatible, and NVIDIA CUDA installation being unintuitive. 

May consider adding a class that will allow for a more intuitive input :)