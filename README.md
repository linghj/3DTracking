# 3DTracking
Supplementary material and code for “Simultaneous Measurement of Three-dimensional Trajectories and Wingbeat Frequencies of Birds in the Field”

Citation: H. Ling, G. E. McIvor, G. Nagy, S. MohaimenianPour, R. T. Vaughan, A. Thornton, and N. T. Ouellette, "Simultaneous measurements of three-dimensional trajectories and wingbeat frequencies of birds in the field," submitted.

Contacts: 
Nicholas Ouellette, Stanford University, nto@stanford.edu
Hangjian Ling, Stanford University, linghj@stanford.edu

The supplementary material and code contains the following items:

1. Folder ‘code’ includes Matlab code to: 
(a) detect birds on images using ‘Step1_BirdDetection.m’; 
(b) reconstruct birds’ 3D locations using ‘Step2_Recon3D.m’. The stereo-matching algorithm solves the optical occlusion problem frame by frame. 
(c) track individuals’ 3D motion using ‘Step3_tracking.m’. The tracking code uses a three-frame predictive particle tracking algorithm that uses estimates of both velocity and acceleration. Details of the algorithm can be found in Ouellette, et al., (2006). A quantitative study of three-dimensional Lagrangian particle tracking algorithms. Experiments in Fluids 40, 301-313.
(d) calculate wing motion and wingbeat frequency from tracking results using ‘Step4_wing.m’.

Sample raw images and the corresponding camera parameters are provided to test these codes. 

2. Folder ‘Data_raw’ includes sample images captured by four cameras. The images from each camera are contained in a separate folder labelled by the camera number, which each contain 110 images (where the background has been removed). The birds are represented by dark pixels on the images. 

The camera parameters for each camera is stored in the file ‘camcoefs.mat’. They are represented by 11 coefficients obtained by direct linear transformation. For more details on the camera calibration method, refer to Theriault, et al., (2014). A protocol and calibration method for accurate multi-camera field videography. Journal of Experimental Biology 217(11), 1843–1848

These raw data can be used to test the Matlab codes. There are 6 trajectories in this dataset. 

3. Folder ‘Data_processed’ includes seven plain text files and corresponding Matlab readable files. They represent 4 isolated pairs of jackdaws, 2 isolated pairs of rooks, and groups of jackdaws. Each text files includes bird id number, positions, times, velocities, accelerations, and wingbeat frequencies at every time step. These data were used to produce the results in the paper. 

4. Folder ‘Results_figures’ includes the corresponding data and Matlab codes needed to reproduce figures 4(a) and 5. Figure 4(a) shows 5 sample trajectories colored with wingbeat frequency. Figure 5 shows the relationship between wingbeat frequency and flight speed. 

5. Folder ‘Results_videos’ includes two videos corresponding to the plain text file named ‘jackdaw_group.txt’. The videos show the time variation of the bird 3D positions. 


