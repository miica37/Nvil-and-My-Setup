###############################
Radial Menus
###############################


.. image:: /images/Radial-menu-list.jpg
	:align: center



***********************
Customize <F9>
***********************

A radial menu for Customize Tools, Customize Radial Menus, Customize Composite Tools and Customize StreamLine Tools.

:kbd:`Shift-Numpad6`

.. image:: /images/Customize-Radial-Menus.gif
	:align: center

.. note::
	Rationale behind using <F9> key: Hmm... Probably took it from XYplorer's (a non-3d application that I am using) hotkey <F9> used for opening its Configuration menu. I think other Functions key (F1-F12) are also fine for the role but instead of assigning one hotkey to each customize window (say <F6> to open up Customize Tools, <F7> to open up Customize Radial Menus and so on), use a radial menu so you only have to remember one hotkey.

************************
Orientation <Ctrl+Space>
************************

A radial menu to set the orientation for Manipulator Tools.

I actually just use Pivot+Orientation(Selection) most of the time, and Orientation(World) on some cases. I think I almost never used the Pivot+Orientation(Object)

.. image:: /images/Orientation-Radial-Menus.gif
	:align: center

.. note::
	Rationale behind using <Ctrl+Space> key: It's after watching `Heavypoly's tutorial <https://www.youtube.com/user/kakapoopie/videos>`_. I saw him using <Space> for a few of his pie menus and thought Hey I could make use of the spacebar too. By the way, he's using <Shift+Space> for his Transforms pie menu, which opens up the menu for orientation, pivots and other stuffs, but I got <Shift+Space> used for Snap View already.


************************
Normals <N>
************************

A radial menu for different Normals related Functions: Harden Selection (set selected components to hard edges), Soften Selection (set selected components to soft edges), Flip Polygon Facing, Unify Polygon Facings, Show Hard Edge Color, Select Hard Edges and Auto Smooth (which is set to an angle of 145).

A few of them are composite tool: Auto Smooth, Harden Selection, Soften Selection. The code blocks below shows how I set them up.

Auto Smooth (Composite Tool)
============================

::

	* Common Modeling Shortcut Tools >> P_AutoSmooth_Whole(*)   Param:Angle(145:00)

Harden Selection
================

The reasons for using a composite tool for this is because Edge Shortcut Tools >> Harden/Soften Selected only works on edge selections, it will do nothing if you have faces selected. The composite tool will help us automate the switching to edge mode.

::

	* Common Modeling Shortcut Tools >> Switch To Edge Mode$
	* Edge Shortcut Tools >> Harden/Soften Selected#


Soften Selection
================

::

	* Common Modeling Shortcut Tools >> Switch To Edge Mode$
	* Edge Shortcut Tools >> Soften/Harden Selected#


.. image:: /images/Normals-Radial-Menus.gif
	:align: center

.. note::
	Rationale behind using <N> key: 'N' for Normals :)

***********************
Context Functions <Tab>
***********************

A radial to...