# 3DTracking
Supplementary code for “Simultaneous Measurement of Three-dimensional Trajectories and Wingbeat Frequencies of Birds in the Field”

Citation: H. Ling, G. E. McIvor, G. Nagy, S. MohaimenianPour, R. T. Vaughan, A. Thornton, and N. T. Ouellette, "Simultaneous measurements of three-dimensional trajectories and wingbeat frequencies of birds in the field," submitted.

Contacts: 
Nicholas Ouellette, Stanford University, nto@stanford.edu
Hangjian Ling, Stanford University, linghj@stanford.edu

The supplementary code contains the following items:

(a) detect birds on images using ‘Step1_BirdDetection.m’; 

(b) reconstruct birds’ 3D locations using ‘Step2_Recon3D.m’. The stereo-matching algorithm solves the optical occlusion problem frame by frame. 

(c) track individuals’ 3D motion using ‘Step3_tracking.m’. The tracking code uses a three-frame predictive particle tracking algorithm that uses estimates of both velocity and acceleration. Details of the algorithm can be found in Ouellette, et al., (2006). A quantitative study of three-dimensional Lagrangian particle tracking algorithms. Experiments in Fluids 40, 301-313.

(d) calculate wing motion and wingbeat frequency from tracking results using ‘Step4_wing.m’.
