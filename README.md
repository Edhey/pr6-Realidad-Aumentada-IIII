# Práctica 6 - Realidad Aumentada

- **Author**: Himar Edhey Hernández Alonso
- **Subject**: Interfaces Inteligentes

## Introducction

In this practice, we will implement a scene in Unity where we will using real-world image targets to place virtual objects in augmented reality. We will use Vuforia as the AR platform to recognize and track images.

## Work Steps

We first need to set up a Unity project with Vuforia:

1. Login in the Vuforia Developer Portal and create a new license key for the project
2. Download and import the Vuforia Engine package into Unity

Then we add the ARCamera prefab to the scene, replacing the default Main Camera, we set the license key in the ARCamera component and create an Image Target database in the Vuforia Developer Portal. Finally, we upload the images you want to use as targets, in this case, we will a image of Rayo McQueen and other of The King both from the movie Cars.
This way we can download the database and import it into Unity. So we can add Image Target prefabs to the scene and set the database and image target for each prefab.

Finally, we add 3D models of a sphere and a cube as children of their respective Image Target prefabs, adding to the the color of each character. We could have used, for example, 3D models of Rayo McQueen and The King, adjusting their position, rotation, and scale to fit the image targets, but as the exercise focuses on basic shapes, we will stick with the sphere and cube.

![Augmented Reality Scene](./Resources/RAScene.gif)