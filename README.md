# Build3dModel
Build 3D model using OpenCV

E was described in almost the exact same words as the homography
matrix H in the previous section. Although both are constructed from similar information, they are not the
same matrix and should not be confused. An essential part of the defi nition of H is that we were considering
a plane viewed by a camera and thus could relate one point in that plane to the point on the camera plane.
Th e matrix E makes no such assumption and so will only be able to relate a point in one image to a line in
the other.

The essential matrix E is purely geometrical and knows nothing about imagers. It relates the location, in physical coordi-
nates, of the point P as seen by the left camera to the location of the same point as seen by the right camera (i.e., it relates p l to p r ). Th e fundamental matrix F relates the points on the image plane of one camera in image coordinates (pixels) to the points on the image plane of the other camera in image coordinates (for which we will use the notation
q l and q r ).

the fundamental matrix F is just like the essential matrix E, except that
F operates in image pixel coordinates whereas E operates in physical coordinates.* Just
like E, the fundamental matrix F is of rank 2. Th e fundamental matrix has seven pa-
rameters, two for each epipole and three for the homography that relates the two image
planes (the scale aspect is missing from the usual four parameters).
