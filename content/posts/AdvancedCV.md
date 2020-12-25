+++
title = "Human 3D Pose Reconstruction"
date = "2020-12-02T16:32:38+01:00"

description = "This lab is about reconstructing joints and displaying them on a video working with different camera angles and therefore transformation matrix and camera intrinsic parameters"
showFullContent = false
+++

Github link for the functions: https://github.com/Foglia-m/AdvancedCV

In this lab, the goal was to implement multi-view reconstruction of the movement using a calibrated system: the joints are already defined with deepnet openpose and must be displayed, frame by frame on each camera image.
Therefore, the idea is to understand the theoretical link between multi-view cameras (rotation and translation matrices) in order to project points from each view into the desired 2D image. 

1. Displaying joints on each frame according to the 2DTXT file.

This is the most trivial process as it only treats the relation between 2D images.
 I coded drawkeypoints.py in order to realise the following: 
	-createframesfrom2Dfile: Take a 2D file as input and extract it into a frames array so that we can display each frame on the corresponding video in the drawing function
	-drawing: takes a videopath and the extracted frames (from createframesfrom2Dfile), uses opencv dedicated functions to draw the junctions on every frame of the video and save it.

This is an example of the basic output of this function using Lea/squat_1_0.0.avi as the videopath and squat_1_0.0.txt as the 2D file.
We can see on this frame that the joint rendering is good: 

![Lea1](/blog/LEA1.jpg)

2. Same goal using the 3DTXT file of an activity and project the 3D reference of the 0 camera into the others.
The tricky part here is to understand the relation between the 3d points of one camera and the 2d points of another camera. We can draw the following pipeline to understand the relation:

a. 3D_coords_cam_0  ⇒ 3D_coords_cam_i  (unhomogenous)
using Transform matrix T(3x4) or (4x4 in homogeneous coord) coming from the pose_0_i.xml file as the transform matrix. 
This matrix contains both rotation and translation so it defines the exact origin shift between both cameras and can therefore be applied to each joint of a frame. 

b. 3D_coords_cam_i ⇒  2D_coords_cam_i
using the intrinsic parameters of the camera from the out_camera_data_i.xml file.
They define the projection from a 3D space to the 2D space of the camera image, therefore, we can retrieve the final coordinates of our joints on the corresponding video.


Code wise, I implemented two functions in a python file called Pose_ProjectFrom3D.PY
This file has the following functions: 
	-Create_frames_list taking the video3D.txt file as input in order to return the 3D_coords_cam_0 objects (the coordinates of the joints according to the 0 camera).
	-Projection_to_cam_i takes as input the frames from the last function and a i index, this index defines the camera we want to treat. We extract the camera pose data in order to compute the 3D_coords_cam_i (a) and then we extract the camera intrinsic data in order to project the 3D new coords in the 2D space. Then we use the drawkeypoints.py method to display the corresponding joints. 

Remark: Here I was stuck because I did not understand why my outputs were bad when I drew on the video, here’s a gif of my output. (the gif does not represent the true number of points as it was locked by framerate, it looks like there is only one point here whereas there were actually plenty of them.  
![unstable](/blog/unstablepoints.gif)

Still, I used the demo.py in order to continue and it worked: 

![khoa1](/blog/khoa1.jpg)

We can see the points correctly follow the joints of the person.

For the triangulation, we can use the demo2.py file, 
we also get good results for the points at each frame:

![Lea2](/blog/LEA2.jpg)

Conclusion: Unfortunately, I was stuck with unstable results with the 3D to 2D part so I could not advance further in the lab. Still I spent a lot of time understanding the different transforms between camera viewpoints (with/without homogeneity of the coordinates) so I managed to work on many things. An interesting subject to me is the calibration of cameras, I would do it using arucos which have interesting geometrical properties and great robustness to angles: 

![arucos](/blog/arucos.png)






