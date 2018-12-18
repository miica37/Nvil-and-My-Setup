###############################
Radial Menus
###############################


.. image:: /images/Radial-menu-list.jpg
	:align: center



*********************************************************************
Customize <F9>
*********************************************************************

A radial menu for Customize Tools, Customize Radial Menus, Customize Composite Tools and Customize StreamLine Tools.

.. image:: /images/Customize-Radial-Menus.gif
	:align: center

.. note::
	Rationale behind using < F9 > key: Hmm... Probably took it from XYplorer's (a non-3d application that I am using) hotkey < F9 > used for opening its Configuration menu. I think other Functions key (F1-F12) are also fine for the role but instead of assigning one hotkey to each customize window (say < F6 > to open up Customize Tools, < F7 > to open up Customize Radial Menus and so on), use a radial menu so you only have to remember one hotkey.

:: _orientation_radial_menu:

*********************************************************************
Orientation <Alt+Q>
*********************************************************************

A radial menu to set the orientation of Manipulator (Gizmo).

I actually just use Pivot+Orientation(Selection) most of the time, and Orientation(World) on some cases. I think I almost never used the Pivot+Orientation(Object)

.. image:: /images/Orientation-Radial-Menus.gif
	:align: center

.. note::
	Rationale behind using < Alt+Q > key: I tried to use < Ctrl + Space > as the hotkey after watching `Heavypoly's tutorial <https://www.youtube.com/user/kakapoopie/videos>`_. I saw him using < Space > for a few of his pie menus and thought I could make use of the spacebar too. He is using < Shift+Space > for his Transforms pie menu, which opens up the menu for orientation, pivots and other stuffs, but I got < Shift+Space > used for Snap View already. I found that < Ctrl + Space > conflict with some other hotkey, so I switched back to < Alt + Q > which I use long time ago.


*********************************************************************
Normals <N>
*********************************************************************

.. image:: /images/Normals-Radial-Menus.jpg
	:align: center

A radial menu for different Normals related Operations: Harden Selection (set selected subobjects to hard edges), Soften Selection (set selected subobjects to soft edges), Flip Polygon Facing, Unify Polygon Facings, Show Hard Edge Color, Select Hard Edges and Auto Smooth (which is set to an angle of 145).

.. admonition:: Reference
	:class: refbox

	:Flip Polygon Facing:      :menuselection:`Geometry --> Common Commands n Tools --> Flip Polygon Facing`

	:Unify Polygon Facings:      :menuselection:`Geometry --> Common Commands n Tools --> Unify Polygon Facing`

	:Show Hard Edge Color:      :menuselection:`View --> Navigation --> Show Hard Edge Color On Unselected`

.. image:: /images/Normals-Radial-Menus.gif
	:align: center

A few of them are composite tool: Auto Smooth, Harden Selection, Soften Selection and Select Hard Edges. The code blocks below shows how I set them up.

Auto Smooth (Composite Tool)
=================================================

::

	 Composite Setup
	-----------------
	* Common Modeling Shortcut Tools -> P_AutoSmooth_Whole(*)
		Param:Angle(145:00)

Harden Selection (Composite Tool)
=================================================

The reasons for using a composite tool for this is because Edge Shortcut Tools -> Harden/Soften Selected only works on edge selections, it will do nothing if you have faces selected. The composite tool will help us automate the switching to edge mode.

::

	 Composite Setup
	-----------------
	* Common Modeling Shortcut Tools -> Switch To Edge Mode$
	* Edge Shortcut Tools -> Harden/Soften Selected#

Soften Selection (Composite Tool)
=================================================

::

	 Composite Setup
	-----------------
	* Common Modeling Shortcut Tools -> Switch To Edge Mode$
	* Edge Shortcut Tools -> Soften/Harden Selected#

Select Hard Edges (Composite Tool)
=================================================

::

	 Composite Setup
	-----------------
	* Common Modeling Shortcut Tools -> Switch To Edge Mode$
	* Edge Shortcut Tools -> Select Hard Edges

.. note::
	Rationale behind using < N > key: 'N' for Normals :)

*********************************************************************
Context Functions <Tab>
*********************************************************************

WIP