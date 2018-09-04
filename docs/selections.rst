###############################
Selections
###############################


.. image:: /images/Selections-list.jpg
	:align: center


*******************
Selection Tools <Q>
*******************

Toggle visibility of Transform Manipulator

.. note::
	Rationale behind using <Q> key: Copy from Maya.


*******************
Loop Select <Alt+E>
*******************

Select loop.

.. image:: /images/Loop-Select.gif
	:align: center


.. note::
	Rationale behind using <Alt+E> key: Silo.

.. note::
	Default Nvil hotkey for Loop Select: Double click on edge


*******************
Ring Select <Alt+R>
*******************

Select ring.

.. image:: /images/Ring-Select.gif
	:align: center

.. note::
	Rationale behind using <Alt+E> key: Silo.

.. note::
	Default Nvil hotkey for this: <H>

******************************
Grow/Shrink Loop Sel <Shift+E>
******************************


.. image:: /images/Grow-Shrink-Loop-Selection.gif
	:align: center

.. note::
	Rationale behind using <Shift+E> key: Following <Alt+E> used in Loop Select.

.. note::
	Default Nvil hotkey for this: <None>


******************************
Grow/Shrink Ring Sel <Shift+R>
******************************

.. image:: /images/Grow-Shrink-Ring-Selection.gif
	:align: center

.. note::
	Rationale behind using <Alt+E> key: Following <Alt+R> used in Ring Select.

.. note::
	Default Nvil hotkey for this: <None>


**********************************************************
Similar Facing <Y> and Similar Facing (Connection) <Alt+Y>
**********************************************************

There are two tools for select subobjects which face roughly in the same direction as the selected/highlighted subobjects. The one without connection will apply selection all through the model, the one with connection will apply selection to connected subobjects. I use the one with connection most of the time, unfortunately it doesn't support threshold adjust with mouse scrolling. So if you need to adjust the threshold without going through Preference Window, you can activate the other Similar Facing first and adjust the value, then switch back to Similar Facing (Connection).

.. image:: /images/Select-Similar-Facing.gif
	:align: center

.. note::
	Rationale behind using <Y/Alt+Y>  key: Nvil actually has a default hotkey for this is which is quite good, but this tool also has an option to let us adjust the threshold value with mouse scrolling up and down, so setting the hotkey to MMB click will prevent us from using that option. If you want to change the threshold you would need to open up the Preference Window and set the value manually (which is not quite intuitive compared to scrolling mouse wheel and seeing changes update in realtime).

	Y is quite an odd choice, and I have no good reasons. It just happens that the hotkeys that are nearest to ASDF (which my fingers are staying on top 99% of the time) are all used up (QWER, ZXCV, T for extrude, G for Grid, B for Bevel), and I don't want to use any modifier keys with it. So I choose 'Y'.

.. note::
	Default Nvil hotkey for this: <Double MMB click the same polygon>


******************************
Invert Selection <Ctrl+I>
******************************

Invert Selection. Hotkey is same as Nvil default. Put here as reference.

****************************
Full Grow Selection <Ctrl+A>
****************************

Grow selection to whole mesh connected with selected subobject. This can also be done with double clicking subobject.

(I was actually looking for a tool that will select all the meshes inside an object though. I will go through this one and might just remove the hotkey for this.)


.. image:: /images/Full-Grow-Selection.gif
	:align: center


****************************
Soft Selection <Alt+Shift+S>
****************************

Soft Selection.

.. image:: /images/Soft-Selection.gif
	:align: center


.. note::
	Rationale behind using <Alt+Shift+S> key: Used to this key coming from Silo.

.. note::
	Default Nvil hotkey for this: Nvil has Modeling Options -> Soft Selection Enabled and <Alt+X1> is its hotkey (I have no idea what is X1 actually). But I am using the StreamLine version: StreamLine Basic Tools -> Generic Tools -> Increase/Decrease Soft Selection

************************
Select Similar <Shift+M>
************************

Nvil: "Select subobjects which have similar shape or surrounding shape to the selected/hilighed subobjects. The shreshold value can be adjusted by WMB while its hotkey is pressed down and the selection will happen in real time."

.. image:: /images/Select-Similar.gif
	:align: center

.. note::
	Rationale behind using <Y/Alt+Y> key: Nvil actually has a default hotkey for this is which is quite good, but this tool also has an option to let us adjust the threshold value with mouse scrolling up and down, so setting the hotkey to MMB click will prevent us from using that option. If you want to change the threshold you would need to open up the Preference Window and set the value manually (which is not quite intuitive compared to scrolling mouse wheel and seeing changes update in realtime).

	Y is quite an odd choice, and I have no good reasons. It just happens that the hotkeys that are nearest to ASDF (which my fingers are staying on top 99% of the time) are all used up (QWER, ZXCV, T for extrude, G for Grid, B for Bevel), and I don't want to use any modifier keys with it. So I choose 'Y'.

.. note::
	Default Nvil hotkey for this: <None>

***************************************
Symmetrize Selection <Ctrl+Alt+Shift+M>
***************************************

Works on symmetry model. Select the same subobjects on different side. Can be useful for marking seams I think, but I haven't have the need to use this tool much yet.

.. image:: /images/Symmetrize-Selection.gif
	:align: center

.. note::
	Rationale behind using <Ctrl+Alt+Shift+M> key: 'M' in 'SyMMetrize', maybe that will makes it easier to remember. It's also using all the 3 modifier keys because I don't remember using this tool much.

.. note::
	Default Nvil hotkey for this: <None>

****************************
Isolate Selection <Numpad />
****************************

Isolate Selection

.. note::
	Rationale behind using <Numpad /> key: Blender.

.. note::
	Default Nvil hotkey for this: <None>
