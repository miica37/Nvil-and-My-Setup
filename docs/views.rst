###############################
Views
###############################


.. image:: /images/Views-list.jpg
	:align: center

.. _snap_view:

*******************************************************************************
Snap View <Shift+Space> and Snap View on Rotating <Shift>
*******************************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu: (NOT FOUND UNDER MENU)
	:Set:      :menuselection:`View Navigation Tools --> Snap View$`
	:Set:      :menuselection:`View Navigation Tools --> Snap View (Orthographic)$`
	:Default Hotkey: < Shift+Space > and < Shift > (NO CHANGE)

Snap View on Rotating is a nice feature that lets you switch to your desired orthographic view intuitively. Lets say you want to switch to front view, orbit your viewport to about the front side of your model and while still holding down the < Alt+LMB >, press < Shift >.. Bam! your view is now snapped to front orthographic view. To get out of it and get back into perspective view, press < Shift+Space >. This feature substitutes the Front, Side, Top functions frequently seen in 3d application and free up the keys to be used for other purposes. There is also no need to remember any keys (other than < Shift >) or use any marking/pie menu.

.. image:: /images/Snap-View.gif
	:align: center

*********************************************************************
Undo View <[> and Redo View <]>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:      :menuselection:`View --> Undo View$`
	:Menu:      :menuselection:`View --> Redo View$`
	:Default Hotkey: < Shift+Z > to undo view and < Ctrl+Y > to redo view.

I haven't found much need to undo and redo my view, but on the occasion when it is needed, having a hotkey for them can be handy.

.. note::
	Rationale behind using < [ > and < ] > key: Carried from Maya.

*********************************************************************
Fog Adjust <Alt+F> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Fog Enabled: :menuselection:`View --> Fog Enabled`
	:Fog Color: :menuselection:`Edit --> Preference --> Colors --> Viewport Colors --> Fog`
	:Set: 3 new basic streamline tool, Adjust FogStart/End/Intensity. :ref:`(See the setup below) <fog_adjust_setup>`
	:Default Hotkey: < None >

Fog is added on `quite recently <http://samardac.com/nvil-forum//index.php/topic,4578.msg17348.html#msg17348>`_ (6th April 2018). I have always felt that material shading in Nvil less appealing than other 3d apps, this feature helps lift up the shadows area to create a softer and nicer look.

Note: < Alt-F > is not a Fog toggle (I created a button for that) but a streamline tool to control Fog's Start, Fog's End and its Intensity.

(For reference, my values for those are FogStart: 0.005, FogEnd: 0.02, FogIntensity: 0.5492. My fog color is set to RGB(145, 167, 176). Color setting for Fog is under Preference > Colors > Viewport Colors.)

Note: Gif animation below shows the difference between having Fog on or off in a scene (not Fog Adjust).

.. image:: /images/Fog.gif
	:align: center

.. _fog_adjust_setup:

Setup for streamline tool:

.. image:: /images/Fog-adjust-setup.jpg

.. note::
	Default Nvil hotkey for this: < None >

*********************************************************************
Zoom Selection <Z>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:      :menuselection:`View --> Viewport Framing --> Best Fit`
	:Default Hotkey:      < F6 > for Best Fit and < F7 > for Best Fit All
		(Note: it is different from Best Fit (All Views) and Best Fit All (All Views))

.. note::
	Rationale behind using < Z > key: Carried from 3ds max. I used to use 3ds max for a short period of time, never get used to it but some jobs require it to be used. < Z > for zoom is a workflow that I really like from 3ds max, because zoom is heavily used and being so close to ASDF, it's super effective.

