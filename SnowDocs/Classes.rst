Classes
+++++++

In this segment, all of the classes that make SnowSoup are explained in great detail in order to make you understand everything one must know to develop a game using this engine.

Node
====
The Node class is the most basic node type in SnowSoup. It's only purpose is to exist inside the SceneGraph of the engine and to have virtual methods that must be implemented by its subclasses. All other nodes are subclasses of this node and implement the Update virtual method.

Transform
=========
This class has the purpose of giving nodes a representation in 3D space. This means it gives a node position, rotation and scale properties. Every node that can move in 3D space is a subclass of this class.

Model
=====
The Model class stores a 3D model of your choosing. The best 3D format for SnowSoup is FBX, also known as .fbx, so make sure to use it. This class inherits from Transform.

Collider
========
The Collider class represents an axis-aligned bounding box that detects collision with other colliders. This class inherits from Transform.

Projection Camera
=================
The projection camera is the node from which the player can see the 3D world. Inherits from Transform.