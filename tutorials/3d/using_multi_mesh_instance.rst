.. _doc_using_multi_mesh_instance:

Using MultiMeshInstance
-----------------------

Introduction
~~~~~~~~~~~~

In a normal scenario you would use a :ref:`MeshInstance <class_MeshInstance>` node to display a 3D mesh like a human model for the main character. But in some cases you would like to create multiple instances of the same mesh in a scene. You *could* duplicate the same node multiple times and adjust the transforms manually. This may be a tedious process and the result may look mechanical. Also, this method is not favourable to rapid iterations. :ref:`MultiMeshInstance <class_MultiMeshInstance>` is one of the possible solutions to this problem.

MultiMeshInstance, as the name suggests, creates multiple copies of a MeshInstance over a surface of a specific mesh. An example would be having a tree mesh populate a landscape mesh with random scales and orientations. 

Setting up the nodes
~~~~~~~~~~~~~~~~~~~~

The basic setup requires three nodes. Firstly, the multiMeshInstance node. Then, two MeshInstance nodes. 

One node is used as the target, the mesh that you want to place multiple meshes on. In the tree example, this would be the landscape.

Another node is used as the source, the mesh that you want to have duplicate. In the tree case, this would be the tree.

In our example, we would use a :ref:`Node <class_Node>` as the root node of the scene. Your scene tree would look like this:

.. image:: img/multimesh_scene_tree.png

.. note:: For simplification purpose, this tutorial would use built-in primitives. 

Now you have everything ready. Select the MultiMeshInstance node and look at the toolbar, you should see an extra button called ``MultiMesh`` next to ``View``. Click it and select *Populate surface* in the dropdown menu. A new window titled *Populate MultiMesh* will pop up.

.. image:: img/multimesh_toolbar.png

.. image:: img/multimesh_settings.png

MultiMesh Settings
~~~~~~~~~~~~~~~~~~

Below are descriptions of the options.

Target Surface
++++++++++++++
The mesh you would be using as the target surface for placing copies of you source mesh on.

Source Mesh
+++++++++++
The mesh you want duplicated on the target surface.

Mesh Up Axis
++++++++++++
The axis used as the up axis of the source mesh.

Random Rotation
+++++++++++++++
Randomizing the rotation around the mesh up axis of the source mesh.

Random Tilt
+++++++++++
Randomizing the overall rotation of the source mesh.

Random Scale
++++++++++++
Randomizing the scale of the source mesh.

Scale
+++++
The scale of the source mesh that will be placed over the target surface.

Amount
++++++
The amount of mesh instances placed over the target surface. 

Select the target surface, in the tree case, this should be the landscape node. And the source mesh should be the tree node. Adjust the other parameters according to your preference. Press ``Populate`` and multiple copies of the source mesh will be placed over the target mesh. If you are satisfied with the result, you can delete the mesh instance used as the source mesh. 

The end result should look like this:

.. image:: img/multimesh_result.png

To change the result, repeat the same step with different parameters.
