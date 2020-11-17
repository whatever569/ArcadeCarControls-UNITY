# ArcadeCarControls-UNITY
Here is a C# script that you can add to any game object to make it have some vehicular controls without the need of wheel colliders

# How to use?
- create a rectangular prism and name it "Car", give it a rigidBody and a collider
- create an empty game object and name it "Ground detector ray", preferably right under your "Car"
- create a new layer named "floor" and make your ground part of that layer
- drop this script onto your "Car", then, drop your "Ground detector ray" in the "Ray Pos" spot, then make the new layer that you made "floor" the "Floor layer"
- *Optional* if you want to use a car model, make that model a child of "Car" and adjust the colliders and the position of the "Ground ray detector" based on your needs
# Default settings (the settings that work)
- rigidBody: mass = 7
- rigidBody: angular drag = 5
- Car script: Y turning constant = 180
- Car script: Default drag = 3
- Car script: In air drag = 0.1
- Car script: Z turning constant = 2.5
- Car script: Ray length = 0.5
- Car script: Force mode for Z turning = Impulse (impulse to flip the car over if upside down)
- Collider type : box collider
- Cube scale : x,y,z : 1, .5, 2

# Notes
- try to read the script and understand it, remove a couple of functions from Update() and FixedUpdate() to see what happens
- controls are : WASD for moving side to side, forwards and backwords : EC for rotating the car in the Z axis (only if the car isn't detecting the ground)
