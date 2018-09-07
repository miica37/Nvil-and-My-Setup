###############################
ZXCV Rows
###############################


.. image:: /images/ZXCV-rows-list.jpg
	:align: center



*********************************************************************
Cut <X> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           (Alternative) :menuselection:`Polygon Shortcut Tools --> Cut`
	:Set:            :menuselection:`StreamLine Engine Tools --> Cut`
	:Usage:          [1] LMB Click upon geometry to start cutting, use LMB to continue normal cutting, use MMB to cut will skip the polygon point, use RMB to cut last point and terminate the cutting, use Caps-Lock to delete splited edges. [2] Drag LMB from empty space to slice without splitting. [3] Drag RMB to slice with splitting. [Note] To slice with Vertical/Horizontal/Cross constraint, press down Shift key. To slice with angle constraint from Angle Stepping setting, press down Ctrl key. While drawing slice line, to move slice line, press down Space key. To move slice line in horizontal/vertical/OwnDirection, use Space+Shift/Ctrl/(Shift+Ctrl).
	:Default Hotkey: < C >

The Swiss Army Knife Cut Tool. The cut tool I know.. coming from Silo, is able to do a few different kind of cuts all in one tool. The very 1st should be the common cut/knife function, besides cutting the polygons in a point and click fasion, we can also 'slice' the polygons by dragging a line across (:ref:`1st gif below <first_cut_function>`). 2ndly, if we have two vertices selected, it should connect/join them, creating an edge in between (:ref:`1st gif below <first_cut_function>`). 3rdly, if we have an edge selected, it should split it into two, creating a vertex in the middle (:ref:`2nd gif below <second_cut_function>`). Finally if we have two edges or more edges which are selected in ring pattern, it should create a edge loop in the edge ring (:ref:`3rd gif below <third_cut_function>`). Those are the primary functions we will often used in poly modeling and they are nicely packed into one hotkey. Nvil even added face selections into its operands (:ref:`4th gif below <fourth_cut_function>`).

.. _first_cut_function:

.. image:: /images/Cut.gif
	:align: center

.. _second_cut_function:

.. image:: /images/Cut-single-edge.gif
	:align: center

.. _third_cut_function:

.. image:: /images/Cut-edge-ring.gif
	:align: center

.. _fourth_cut_function:

.. image:: /images/Cut-faces.gif
	:align: center

.. note::
	Rationale behind using < X > key: Carried from Silo.

.. _combine:

*********************************************************************
Combine Mesh <Ctrl+Shift+C>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Combine(Merge Meshes)`
	:Default Hotkey: < None >
	:Related:        :ref:`Split Mesh <split_mesh>`

Combine two or more objects into one.

.. note::
	Rationale behind using < Ctrl+Shift+C > key: 'C' for Combine!

*********************************************************************
Circularize <Alt+C> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :(NOT FOUND UNDER MENU)
	:Set:            :menuselection:`StreamLine Basic Tools --> Subobject Tools --> Circularize_Selection`
	:Usage:          On mouse button pressed down, the program will attemp to circularize any selection. To control the orientation, place cursor near a target vertex before starting. If saved transform is presented, it will be used to conrol the deforming. In edge mode, if there is no selection suitable for circularizing, the program will attempt to select an edge loop from the highlighted edge and circularize it. To toggle surface style, tap Caps-Lock key. After circularizing, drage mouse to scale, Space+drag to rotation selection. To toggle spacing style, tap Enter key. To cycle edge circle loop direction, tap Alt key.
	:Default Hotkey: < None >

Circularize selection.

.. image:: /images/Circularize.gif
	:align: center

.. note::
	Rationale behind using < Alt+C > key: 'C' for Circle!

*********************************************************************
Loop Cut <Shift+C> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :(NOT FOUND UNDER MENU)
	:Set:            :menuselection:`StreamLine Engine Tools --> Loop Cut/Slide Edges`
	:Default Hotkey: < S >

.. image:: /images/Loop-Cut.gif
	:align: center

I made some slight changes to the Loop Cut that comes with Nvil. I switch Edge_Loop_Cut/Slide_Proportional with Slide_EdgeMidPoint because often I want the loop to be created in the middle, Slide_Proportional have no way to do that. If I want a proportional loop, I can also achieve with Slide_EdgeMidPoint by click and drag. Basically, Slide_EdgeMidPoint is 2 in 1, while Slide_Proportional is just 1. Then I added Edge_DoubleLoop_Cut/Slide, which is quite useful too in subdivision modeling, for creating control egde loops.

.. image:: /images/Loop-Cut-streamline-modification.jpg
	:align: center

.. note::
	Rationale behind using < Shift+C > key: 'C' for Cut! Actually.. I should be using < Shift+X > because that's what Silo is using, but.. I am not sure why at some point I changed to this hotkey and my muscle memory have adapt to < Shift+C > already. So I will leave it like that.

.. _split_mesh:

*********************************************************************
Split Mesh <Ctrl+B>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Common Commands n Tools --> Split`
	:Default Hotkey: < None >
	:Related:        :ref:`Combine Mesh <combine>`

The reverse of :ref:`Combine <combine>`.

.. image:: /images/Split-Mesh.gif
	:align: center

.. note::
	Rationale behind using < Ctrl+B > key: 'B' for Break! (Break == Split in Silo) Copied from Silo.

*********************************************************************
Bevel <B> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Subobject
	:Menu:           (Alternative) :menuselection:`Geometry --> Chamfer`
	:Default Hotkey: < None >

.. image:: /images/Bevel.gif
	:align: center

.. note::
	Rationale behind using < B > key: 'B' for Bevel! Copied from Silo too.


*********************************************************************
Unchamfer <Alt+B>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Polygon
	:Menu:           :menuselection:`Geometry --> Unchamfer`
	:Default Hotkey: < None >

.. image:: /images/Unchamfer-example.jpg
	:align: center

`Added recently <http://samardac.com/nvil-forum//index.php/topic,4719.0.html>`_. I am still not familiar with it, so gif animation below is a simple look of it.

.. image:: /images/Unchamfer.gif
	:align: center

.. note::
	Rationale behind using < Alt+B > key: Following hotkey for Bevel.

*********************************************************************
Bridge <Shift+B> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Edge
	:Menu:           :menuselection:`Geometry --> Bridge`
	:Default Hotkey: < D >. This is actually a complex streamline tool (StreamLine Engine Tools -> Bridge/BridgeHoles/CapHole) different from my setup.

Simple Bridge to create a bridge of polygons between two or more edges. There is also a bridge tool for polygon but I am not familiar with it.

**Note:** At the start of gif animation, I tap < Shift+B > to do a simple bridge. A simple bridge is what I use most often. Then to show the extra features of streamline bridge, I hold down < Shift+B >, < Hold left click >, release < Shift+B >, scroll mouse wheel to add segments, then hit < Space > to switch between linear and curve type, and finally < Hold Caps Lock > and scroll mouse wheel to adjust curve strength.

.. image:: /images/Bridge.gif
	:align: center

.. note::
	Rationale behind using < Shift+B > key: 'B' for Bridge! Copied from Silo too.

*********************************************************************
Draw Mesh <M> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Combine(Merge Meshes)`
	:Default Hotkey: < None >

Draw mesh is a tool for retopo. Istonia have also created `a guide <http://samardac.com/nvil-forum//index.php/topic,4779.msg17637.html>`_ on the forum. To learn how to use this tool, check out `RubberDuck's detailed tutorial on Youtube <https://www.youtube.com/watch?v=5KKrqfK5mk4>`_ and see this tool in action in his `walkthrough of retopo a snail <https://www.youtube.com/watch?v=44ndpC8lMO0>`_

.. raw:: html

	<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
		<iframe src="https://www.youtube.com/embed/wyqukJQPFU8" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
	</div>

	<p>&nbsp;</p>

It is also probably the most complex tools to master in Nvil...

.. image:: /images/Draw-mesh-usage.gif
	:align: center

.. note::
	Rationale behind using < M > key: 'M' in 'Mesh'...

*********************************************************************
Spin Edge </>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Spin --> Spin Edge CCW`
	:Default Hotkey: < None >

.. image:: /images/Spin-Edge.gif
	:align: center

.. note::
	Rationale behind using < / > key: Copied from Silo.
