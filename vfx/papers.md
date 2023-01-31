# Terminology from papers - NERFS

## novel view synthesis

## scene representation

## Camera poses

Angle of the camera when taking a photo

## depth supervision

Providing additional depth information to the ML model. Techniques include LIDAR, stereo matching, Structure from Motion [SfM] like COLMAP

## self-occlusion

When parts of a 3d objects are hidden by other parts of the same object

## RGB-D

RGB + Depth

## KL divergence

Kullback-Leibler divergence (relative entropy) statistical distance between two probability distributions

## Scene composition

Scene composition refers to the way objects and their relationships are arranged within a scene.

## Octree

Data structure used to represent 3D space. It divides space into smaller and smaller regions, known as voxels, until each voxel contains only a single object or data point.

## Signed Distance Function (SDF)


## Spherical harmonics

function defined on the surface of the sphere

## Trilinear interpolation

a method of multivariate interpolation on a 3D regular grid

## Interpolation

a type of estimation, a method of constructing (finding) new data points based on the range of a discrete set of known data points

## Lambertian material

Material that nicely diffuses light and doesn't create reflections. The brightness of such material is the same regardless of an angle. Ideal for mattes.

## Local Light Field Fusion by Mildenhall at el.

Paper proposing reduction of number of training images without quality loss via:
- by estimating amount of "depth" in the image it guides use about how many pictures to take of the scene
- it is also handling light propagation better with merging local light field of adjescent images during inference.

## Light field

A way to represent amount of light in a scene that is incoming in every direction at every point in space. 

## Plenoptics

Capturing and processing the light field of a scene. Combines principles of optics and CG

## CGI

Computer generaterd imaginery

