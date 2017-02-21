<p>An implementation of an inverse perspective mapper using OpenCV functions. To make it work better, there is a couple of things to do:
<ul>
<li>Generate two paris of correspondences on the longitudinal
lane-markings: Deploy a lane-marking detector and use points on the
detected lane-markings. This would give a better, planar homography matrix.
<li>Unit test: If necessary.
</ul>
</p>