###############################
QWERT Rows
###############################


.. image:: /images/QWERT-rows-list.jpg
	:align: center



***********************
Quad Cap <Ctrl+Shift+Q>
***********************

::

	Geometry > Common Commands n Tools > Quad Cap

Quoted from Nvil: "Create quad polygons to fill holes. The number of border edges must be even. Selections must be made to mark two ajacent corners."

Quad Cap is a nice feature of Nvil that has been around for a long time. Back then Nvil has many cool features that Maya doesn't have and this is one of it. To use it you can select just two edges (I selected a loop of edges in the gif animation, that is also ok).

.. image:: /images/Quad-Cap.gif
	:align: center

.. note::
	Rationale behind using <Ctrl+Shift+Q> key: 'Q' for Quad :) Using two modifier keys instead of one because I only use this occasionally.

.. note::
	Default Nvil hotkey for this: <None>

*****************
Make Quad <Alt+Q>
*****************

::

	StreamLine Basic Tools -> Polygon Tools -> Make Quad

This is a streamline tool to convert selected polygon into quads. It has a bit of draw back as seen in the gif animation below, I can't get the pattern I want for the middle one. There's also no option to rotate the generated quad pattern which can be useful for the third circle example.

Nvil: "Press down mouse button to convert polygon selection into quad polygons then drag to adjust orienation. To change row setting, WMB/Alt+drag. To change auto relax option, tap Space key."

.. image:: /images/Make-Quad.gif
	:align: center

.. note::
	Rationale behind using <Alt+Q> key: 'Q' for Quad again!

.. note::
	Default Nvil hotkey for this: <None>

*******************
Vertex Weld <Alt+W>
*******************

::

	StreamLine Basic Tools -> Vertex Tools -> Vertex_Weld

This is a built-in streamline tool to weld vertex one by one. Compared to what I have been used to, this tool makes vertex welding even more streamlined. Before this, my workflow would be select a vertex, then select another vertex and hit a key (<Alt+D> Collapse) to weld first vertex to second vertex. Now, there's no need to select anything, notice in the gif animation I didn't perform any mouse click at all. I hover cursor to the first vertex, press hotkey, move cursor to second vertex, release hotkey, done! This makes welding a row or a bunch of vertices a piece of cake.

Nvil: "Weld vertex to one of its adjacent vertices, or weld two open vertices. Click to pick the first vertex, if mapped to NMB the program will pick up the highlighted vertex as first vertex on activation. Then move cursor over to the second vertex, click or release hotkey to weld."

.. image:: /images/Vertex-Weld.gif
	:align: center

.. note::
	Rationale behind using <Alt+W> key: 'W' for Weld.

.. note::
	Default Nvil hotkey for this: <S>. It is under Built-in Tools > S Tools > Weld Vertex (Vertex)

************************
Threshold Weld <Shift+W>
************************

::

	StreamLine Basic Tools -> Subobject Tools -> Threshold_Weld (Vertex)

This is a streamline tool to weld selected vertices with an option to control threshold by dragging. We can now adjust the threshold in realtime (How cool is that!)

Nvil: "Press down mouse button then drag to adjust weld threshold value. Welding will be performed base on threshold value within subobject selections."

To weld a bunch of vertices that are sitting on top of each other, activate hotkey and instead of click and drag, just click and release to perform a zero threshold weld.

.. warning::
	In Blender, there is Remove Doubles and I half expect this tool to work the same but it won't remove edges and faces that sits on top of each other.

.. image:: /images/Threshold-Weld.gif
	:align: center

.. note::
	Rationale behind using <Alt+W> key: 'W' for Weld.

.. note::
	Default Nvil hotkey for this: <None>

***************************
Weld Options <Ctrl+Shift+W>
***************************

::

	Subobject Shortcut Tools -> Weld

Opens up Weld Options. I used to use Weld Options more often, until Threshold Weld is added.

.. image:: /images/Weld-option.jpg
	:align: center

.. note::
	Rationale behind using <Ctrl+Shift+W> key: 'W' for Weld. Using two modifier keys instead of one because I only use this occasionally.

.. note::
	Default Nvil hotkey for this: <None>

***********
Extrude <T>
***********

Nvil has extrude in its Polygon Shortcut Tools and StreamLine Tools. The streamline version is more versatile as it can act on different subobject mode and for each subjobject mode, we can have different type of extrude on each separate mouse button. Nvil default extrude tool can be accessed from Visual Tool Window or using the default hotkey <A> to activate the streamline version. You can expect it to behave like the extrude tool of other 3d applications. It supports vertex, edge and face.

Since Nvil's doesn't support floating vertex and edge, you can't extrude vertex like Blender. Nvil's Vertex_Extrude (a StreamLine Tool) is a bit different as you can see on the first gif below. Notice that I don't have to click on the vertex, I hover my mouse over to hightlight the vertex and use hotkey <T> to act on it. I guess this can be useful when doing a retopo.

For Edge Extrude, I did some modifications to the original (refer to the :ref:`setup image <extrude_setup>` below). The default setup has only Edge_Extrude_CursorDirection mapped to NMB and LMB (and Edge Shortcut Tools >> Extrude mapped to Redirect). Since I find extruding edge with NMB behaviour are not what I want 99% of the time, I clear the NMB (otherwise everytime you activate the tool and acidentally/instinctly move the mouse, unwanted edge will appears). I mapped Edge_Extrude_Shoulder_Style to MMB because I find it interesting (but I am not sure when should I use this type of extrusion). I mapped Edge_Extrude_Face/Normal_Direction to RMB. Edge_Extrude_Face/Normal_Direction can be really nice on many situations, second gif below is specifically about it.

Another modification I added is Extrude Edge Zero and Extrude Face Zero, and mapped them to On Tapped. Both are composite tool that I created because I cannot find a way to achieve zero length extrude with built-in tools. They are often used when you want to manually translate the extruded suboject using Manipulator. For example, with an edge selected, tap <T> key, another edge will be created on top of the selected one, then you can use any transformation tools to move, scale or rotate the edge.

.. image:: /images/Vertex-extrude.gif
	:align: center

.. image:: /images/Edge-extrude-normal-direction.gif
	:align: center

.. _extrude_setup:

Setup for streamline tool (Subobject Toolset):

.. image:: /images/Extrude-setup.jpg

.. note::
	Rationale behind using <T> key: Extrude is heavily used, so I don't want to use any modifier keys with it; it has to be very close, looking at ASDF, QWER and ZXCV, they have been occupied. The next nearest option would be <T>, <G> and <B>... so <T> is chosen. Actually I think <Alt+E> is also fine, I used to set it to that, maybe I should consider changing it back to <Alt+E> because Blender use <E> too.

.. note::
	Default Nvil hotkey for this: <A>

*********
Inset <I>
*********

Nvil also has inset in its Polygon Shortcut Tools and StreamLine Tools. 

.. note::
	Rationale behind using <I> key: 'I' for Inset :)

.. note::
	Default Nvil hotkey for this: <S>
