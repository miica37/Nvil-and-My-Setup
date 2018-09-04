###############################
Pivots
###############################


.. image:: /images/Pivots-list.jpg
	:align: center

Quote from Nvil Help: "Object pivot is the origin of its base matrix"

These are the streamline tools to manipulate pivots for object and subobjects. They come built-in with Nvil, however it seems no hotkeys are assigned to them yet.

************************
Set Manipulator <Insert>
************************

You can find this tool in StreamLine Tools, it is under Built-in Tools. It is best used with snapping turned on.

.. image:: /images/Set-Manipulator.gif
	:align: center

Note: The followings are from Nvil's Help:

Set manipulator Manually. Possible ways:

1. Use manipulator with LMB to transform.
2. Click to pick the aligning axis (exclude LMB). Move cursor over to a snapping target, LMB/MMB click. For LMB, the rotation axis will be the manipulator's axis that is most parallel to cameral direction. For MMB, the rotation axis will be formed from the plane defined by hilighted axis and snap point.
3. LMB click a snapping target to snap manipulator location onto the snapping point.
4. MMB click a snapping target to snap manipulator orientation onto the snapping point's orientation.
5. RMB click a snapping target to snap manipulator's both loaction and orientation onto the snapping point's loaction and orientation.

Note: If there is no snapping target detected on mouse down, workplane or world's origin and orientation will be used as snapping target. Also in this case, LMB+RMB can be used to set manipuplator location to selection center. (End of Nvil's Help)

.. note::
	Rationale behind using <Insert> key: Coming from Maya, this key is what they use and I don't have much trouble remember it too. Insert also doesn't seem to be used by anything. It's positioned quite far away though. Actually before this, I use <'> (or <.>?), I can remember the key fairly well when I use Nvil more often, but when I take a long break from Nvil, I would get confused by those <'>, <,>, <.> keys... so just trying out a different one.

.. note::
	Default Nvil hotkey for this: <None>

****************************
Obj/Mesh Pivot <Ctrl+Insert>
****************************

You can find this tool in StreamLine Tools, it is under Built-in Tools. It is best used with snapping turned on.

This tool is commonly used when you import an object, and see the object's pivot is set to world center. To center pivot back to the object, hold down <Ctrl+Insert>, hold down left click, then right click to end the operation.

This is just the object/mesh version of the above with a slight difference: "On LMB and MMB down, pivot will snap to object's bounding box center."

.. image:: /images/ObjMesh-Pivot.gif
	:align: center

Note on the gif: At the end, after I set object pivot to the front face, it might not be obvious, I then hold down <Ctrl+Insert>, hold down left click and do a right click to reset pivot back to center of the mesh. Notice that the orientation of pivot is still not same with the world, because the previous function only reset position. You can use Common Modeling Shortcut Tools -> Freeze Object Orientation, that will reset the pivot's orientation back to world space.

.. note::
	Rationale behind using <Ctrl+Insert> key: I choose this one to be the 'Ctrl' version (instead of the quicker <Insert>) because I think I could be using this less often.

.. note::
	Default Nvil hotkey for this: <None>
