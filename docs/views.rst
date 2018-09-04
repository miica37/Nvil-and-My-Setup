###############################
Views
###############################


.. image:: /images/Views-list.jpg
	:align: center

.. _snap_view:

**********************************************************
Snap View <Shift+Space> and Snap View on Rotating <Shift>
**********************************************************

::

	View Navigation Tools -> Snap View$
	View Navigation Tools -> Snap View (Orthographic)$

Snap View on Rotating is a nice feature that lets you switch to your desired orthographic view intuitively. Lets say you want to switch to front view, orbit your viewport to about the front side of your model and while still holding down the <Alt+LMB>, press <Shift>.. Bam! your view is now snapped to front orthographic view. To get out of it and get back into perspective view, press <Shift+Space>. This feature substitutes the Front, Side, Top functions frequently seen in 3d application and free up the keys to be used for other purposes. There is also no need to remember any keys (other than <Shift>) or use any marking/pie menu.

.. image:: /images/Snap-View.gif
	:align: center

.. note::
	Default Nvil hotkey for this: Nvil comes with the same hotkeys so just use it right away :)

*******************************
Undo View <[> and Redo View <]>
*******************************

::

	Common Shortcut Tools -> Undo View
	Common Shortcut Tools -> Redo View

I haven't found much need to undo and redo my view, but on the occasion when it is needed, having a hotkey for them will be handy.

.. note::
	Rationale behind using <[> and <]> key: Copied from Maya.

.. note::
	Default Nvil hotkey for this: <Shift+Z> to undo view and <Ctrl+Y> to redo view.


******************
Fog Adjust <Alt+F>
******************

::

	* View > Fog Enabled.
	* Edit > Preference > Colors > Viewport Colors > Fog.
	* 3 new basic streamline tool, Adjust FogStart/End/Intensity.

Fog is added on `quite recently <http://samardac.com/nvil-forum//index.php/topic,4578.msg17348.html#msg17348>`_ (6th April 2018). I always felt Nvil shading is a bit harsh compared to other 3d applications, this feature helps lift up the shadows area to create a softer and nicer looks. I have Fog turned on always. <Alt-F> is not a toggle on and off for Fog (I created a button for that) but a streamline tool to control Fog's Start, Fog's End and its Intensity.

(For reference, my values for those are FogStart: 0.005, FogEnd: 0.02, FogIntensity: 0.5492. My fog color is set to RGB(145, 167, 176). Color setting for Fog is under Preference > Colors > Viewport Colors.)

.. image:: /images/Fog.gif
	:align: center

Setup for streamline tool:

.. image:: /images/Fog-adjust-setup.jpg

.. note::
	Default Nvil hotkey for this: <None>

******************
Toggle Grid <G>
******************

::

	Common Shortcut Tools -> Toggle Grid Visibility

Toggle Grid on the viewport.

.. note::
	Rationale behind using <G> key: 'G' for Grid :) I believe 3ds max is also using the same hotkey (but I don't use 3ds max anymore though).

.. note::
	Default Nvil hotkey for this: <None>

************
Zoom Sel <Z>
************

::

	View Navigation Tools -> Best Fit

.. note::
	Rationale behind using <Z> key: 3ds max. I used to use 3ds max for a short period of time, never get used to it but some jobs require it to be used. <Z> for zoom is a workflow I really like from 3ds max, because it's so close to ASDF and I use it frequently.

.. note::
	Default Nvil hotkey for this: <F6> for Best Fit and <F7> for Best Fit All (Note: it is different from Best Fit (All Views) and Best Fit All (All Views))



