###############################
Selections
###############################


.. image:: /images/Selections-list.jpg
	:align: center


*********************************************************************
Selection Tool <Q> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Default Hotkey: <Q>

Selection Tool comes as a StreamLine tool. It has 3 functions mapped to the 3 mouse buttons. The first is a lasso selection, second one is lasso selection with raycast, third one is rectangle selection with raycast (See the setup below). Tap <Q> to toggle visibility of transforms Manipulator.

Default setup for Selection Tool (NO CHANGE):

.. image:: /images/Selection-Tool-setup.jpg


*********************************************************************
Loop Select <Alt+E>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode: Subobject
	:Menu:   :menuselection:`Selection --> Loop Select`
	:Default Hotkey: <Edge> Double click an edge; <Face> Select a face, < Ctrl+Shift > double click on an adjacent face; <Vertex> Select a vertex, < Ctrl+Shift > double click on an adjacent vertex

Select loop. Works on vertex, edge and face mode. Actually you don't need to use hotkey for this because double click can also achive the same thing.

.. image:: /images/Loop-Select.gif
	:align: center


.. note::
	Rationale behind using < Alt+E > key: Carried from Silo.

*********************************************************************
Ring Select <Alt+R>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode: Subobject
	:Menu:   :menuselection:`Selection --> Ring Select`
	:Default Hotkey: < H >

Select ring. Works on vertex, edge and face mode. 

.. image:: /images/Ring-Select.gif
	:align: center

.. note::
	Rationale behind using < Alt+E > key: Carried from Silo.

*********************************************************************
Grow/Shrink Loop Sel <Shift+E>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           (NOT FOUND UNDER MENU)
	:Set:            :menuselection:`Subobject Shortcut Tools --> Grow/Shrink Loop Selection`
	:Usage:          "Once hotkeys pressed, scroll WMB up/down to perform action."
	:Default Hotkey: < None >

.. image:: /images/Grow-Shrink-Loop-Selection.gif
	:align: center

.. note::
	Rationale behind using < Shift+E > key: Following < Alt+E > used in Loop Select.

*********************************************************************
Grow/Shrink Ring Sel <Shift+R>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           (NOT FOUND UNDER MENU)
	:Set:            :menuselection:`Subobject Shortcut Tools --> Grow/Shrink Ring Selection`
	:Usage:          "Once hotkeys pressed, scroll WMB up/down to perform action."
	:Default Hotkey: < None >

.. image:: /images/Grow-Shrink-Ring-Selection.gif
	:align: center

.. note::
	Rationale behind using < Alt+E > key: Following < Alt+R > used in Ring Select.

*******************************************************************************
Similar Facing <Y> and Similar Facing (Connection) <Alt+Y>
*******************************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Subobject
	:Menu:           :menuselection:`Selection --> Similar Selection --> Select Similar Facing`
	:Menu:           :menuselection:`Selection --> Similar Selection --> Select Similar Facing(Connection Only)`
	:Usage:          "Select subobjects which Face roughly in the same direction as the selected/hilighed subobject. The threshold value can be adjusted WMB while its hotkey is pressed down and the selection will happen in real time."
	:Default Hotkey: < Double MMB click the same polygon >

There are two tools for select subobjects which face roughly in the same direction as the selected/highlighted subobjects. The one without connection will apply selection all through the model, the one with connection will apply selection to connected subobjects. I use the one with connection most of the time, unfortunately it doesn't support threshold adjust with mouse scrolling. So if you need to adjust the threshold without going through Preference Window, you can activate the other Similar Facing first and adjust the value, then switch back to Similar Facing (Connection).

.. image:: /images/Select-Similar-Facing.gif
	:align: center

.. note::
	Rationale behind using < Y/Alt+Y >  key: Nvil actually has a default hotkey for this is which is quite good, but this tool also has an option to let us adjust the threshold value with mouse scrolling up and down, so setting the hotkey to MMB click will prevent us from using that option. If you want to change the threshold you would need to open up the Preference Window and set the value manually (which is not quite intuitive compared to scrolling mouse wheel and seeing changes update in realtime).

	Y is an odd choice, I have no good reason to use this key. It just happens that the hotkeys that are nearest to ASDF (which my fingers are staying on top 99% of the time) are all used up (QWER, ZXCV, T for extrude, G for Move(Grab), B for Bevel), and I don't want to use any modifier keys with it. So I choose 'Y'.

*********************************************************************
Invert Selection <Ctrl+I>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode: Subobject
	:Menu:   :menuselection:`Selection --> Inverse Selection`
	:Default Hotkey: < Ctrl+I >

*********************************************************************
Select All <Ctrl+A> (Composite Tool)
*********************************************************************

When an object is composed of multiple separate meshes (geometry islands), this tool helps select all the meshes. I couldn't find a tool to do this in Nvil so I created a composite tool.

.. image:: /images/Select-All.gif
	:align: center

::

	 Composite Setup
	-----------------
	* Common Modeling Shortcut Tools -> Save Object Selection Mode^
	* Subobject Shortcut Tools -> P_Math Select Vertices With Edges(*)
		Params: LargerTan(true); Value(1)
	* Common Modeling Shortcut Tools -> Restore Object Selection Mode^

*********************************************************************
Soft Selection <Alt+Shift+S> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode: Subobject
	:Menu:   :menuselection:`Edit --> Options --> Soft Selection Options --> Soft Selection Enabled`
	:Default Hotkey: < Alt+X1 > (I haven't found out what X1 is, but I am using the StreamLine version: StreamLine Basic Tools -> Generic Tools -> Increase/Decrease Soft Selection)

Soft Selection.

.. image:: /images/Soft-Selection.gif
	:align: center


Setup for streamline tool:

.. image:: /images/Soft-Selection-setup.jpg

.. note::
	Rationale behind using < Alt+Shift+S > key: Carried from Silo.

*********************************************************************
Select Similar <Shift+M>
*********************************************************************
.. admonition:: Reference
	:class: refbox

	:Mode:           Subobject
	:Menu:           :menuselection:`Selection --> Similar Selection --> Select Similar`
	:Usage:          "Select subobjects which have similar shape or surrounding shape to the selected/hilighed subobjects. The threshold value can be adjusted by WMB while its hotkey is pressed down and the selection will happen in real time."
	:Default Hotkey: < None >

.. image:: /images/Select-Similar.gif
	:align: center

.. note::
	Rationale behind using < Shift+M > key: WIP

*********************************************************************
Symmetrize Selection <Ctrl+Alt+Shift+M>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Subobject
	:Menu:           :menuselection:`Selection --> Symmetry Selection --> Symmetrize Selection`
	:Default Hotkey: < None >

Works on symmetry model. Select the same subobjects on different side. Can be useful for marking seams I think.

.. image:: /images/Symmetrize-Selection.gif
	:align: center

.. note::
	Rationale behind using < Ctrl+Alt+Shift+M > key: 'M' in 'SyMMetrize', maybe that will makes it easier to remember. It's also using all the 3 modifier keys because I don't remember using this tool much (yet).

*********************************************************************
Isolate Selection <Numpad />
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:   :menuselection:`Selection --> Isolate Selection`
	:Default Hotkey: < None >

Isolate Selection

.. note::
	Rationale behind using < Numpad / > key: Immitate Blender
