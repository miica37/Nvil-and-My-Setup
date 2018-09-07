###############################
ASDF Rows
###############################


.. image:: /images/ASDF-rows-list.jpg
	:align: center


*********************************************************************
Vertex/Edge/Face/Object Mode <A/S/D/F>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           Selection > Selection Modes > Vertex/Edge/Polygon/Object Mode
	:Default Hotkey: < 1/2/3/4 >

One of the most heavily used operation in poly modeling is no doubt switching between subobject modes. Back in the days when I still use Maya, I found this little 3d modeling application called Silo and one of the workflow it introduce is using ASDF to switch between subobject modes. It's been a long time now, I think at first it takes a bit of time to get used to, maybe a few days or a week? I can't remember but I got used to it. I have ever since stubbornly refused to use any other approach.

You can try out other approach like radial menu (Maya style) or the < 1/2/3/4 > keys combination (Nvil Default, `Blender 2.8 too it seems <https://developer.blender.org/T55162>`_). I don't prefer < 1/2/3/4 > though because you need to move your left hand to reach it and move it back to ASDF.

Marking Menus (Maya)
====================

.. image:: /images/Maya-marking-menu.jpg
	:align: center

Maya's default marking menu to switch between subobject modes is really fast (see first gif below), the only problem is it's a tiny bit crowded, I would occasionally get the wrong one between Object Mode and UV, but that wasn't a big deal. You can also use radial menu in Nvil. Nvil's user interface overall is a bit slow on my machine, so there's a bit of lag (see second gif below).


.. image:: /images/Maya-marking-menu-response.gif
	:align: center

.. image:: /images/Nvil-radial-menu-response.gif
	:align: center

*********************************************************************
Relax <Alt+S> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           Geometry > Common Commands n Tools > Relax
	:Set:            :menuselection:`StreamLine Basic Tools -> Generic Tools -> Relax`
	:Default Hotkey: < H > (but only works on Vertices)

Relax (ie. Smooth) in Nvil has a nice touch due to it being a StreamLine tool, ie. you can control how much you want to smooth by how far you drag your mouse, this allows for very fine smooth in one single operation (no need to adjust it by using properties box like in other 3d applications!) Alternatively if you want to smooth it step by step, you can also tap hotkey. Relax is very much used in organic modeling.

.. image:: /images/Relax.gif
	:align: center

Setup for streamline tool (Generic Tool):

.. image:: /images/Relax-setup.jpg

.. note::
	Rationale behind using < Alt+S > key: 'S' for Smooth!

*********************************************************************
Delete <Ctrl+Shift+D> and <Delete>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Common Commands n Tools --> Delete`
	:Default Hotkey: < Delete >

Delete. I have setup another key for this.

.. note::
	Rationale behind using < Ctrl+Shift+D > key: Delete is also a heavily used operation. Unfortunately, < Delete > (or < Backspace >) is a bit far, that means you have to move your hand to reach it. One day I found that the idea to use < Ctrl+Shift+D >, I tried it, it is faster than < Delete > and it felt right. < X > can also be a good candidate, but the place has been taken by Cut Tool.

*********************************************************************
Duplicate <Ctrl+D>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Common Commands n Tools --> Duplicate`
	:Default Hotkey: < Ctrl+D >

Duplicate object and also face.

*********************************************************************
Linear Duplicate <Shift+D> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           (NOT FOUND UNDER MENU)
	:Set:            :menuselection:`StreamLine Basic Tools --> Generic Tools --> Linear Duplicate`
	:Default Hotkey: < None >

I just found out about this tool and will experiment with it for some time.

.. note::
	Rationale behind using < Shift+D > key: experiment

*********************************************************************
Collapse <Alt+D>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Common Commands n Tools --> Collapse`
	:Default Hotkey: < None >

Collapse selected subobjects. Another heavily used tool especially when cleaning up and reducing polygons.

.. image:: /images/Collapse.gif
	:align: center

.. note::
	Rationale behind using < Alt+D > key: I imagining collapsing as deleting some subobjects. As I use this quite often too, 'Alt+D' is a nice position to execute this quickly.

*********************************************************************
Flatten <Ctrl+F>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Common Commands n Tools --> Flatten`
	:Default Hotkey: < None >

Flatten selected subobjects. Can be useful in some situations.

.. image:: /images/Flatten.gif
	:align: center

.. note::
	Rationale behind using < Ctrl+F > key: 'F' for Flatten! (Not carried from Silo which is using < Alt+Shift+F >)

*********************************************************************
Cap Hole <Shift+F>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:`Geometry --> Cap Hole --> Simple`
	:Default Hotkey: Nvil's doesn't have a default hotkey for Cap Hole Simple, but a more complicated streamline tool with hotkey < D > has a CapHole function. It is a combination of Bridge, Bridge Hole and Cap Hole. To cap a hole, you hit < D > and < Double RMB click > on an edge. Most of the time though.. I just need a simple fill, so select and edge and < Shift+F > will do.

Cap Hole (or Fill Hole).

.. image:: /images/Cap-Hole.gif
	:align: center

.. note::
	Rationale behind using < Shift+F > key: 'F' for Fill! Carried from Silo.

*********************************************************************
Slide <J> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           (NOT FOUND UNDER MENU)
	:Set:            :menuselection:`StreamLine Basic Tools --> Subobject Tools --> Slide Seletion`
	:Default Hotkey: < V > and < Middle Click Drag >. This streamline tool is called Tweak_PickThrough/Slide Selection. The Tweak function activated by left and right mouse button seems surprisingly intuitive, and a good combination.. at first... after playing with it for a while, I found a problem. If you use its Tweak function, it will makes soft selection on subobjects and it can't be canceled (even with Soft Selection Window), until you make a new selection. That means if you want to proceed to Slide, without soft selection, you have to click on a empty area to deactivate the soft selection, then only can you slide.

Slide vertices, edges and faces.

.. image:: /images/Slide.gif
	:align: center

.. note::
	Rationale behind using < J > key: Carried from Silo.

*********************************************************************
Shell <K> (StreamLine Tool)
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Menu:           :menuselection:Geometry --> Common Commands n Tools --> Shell
	:Set:            :menuselection:`StreamLine Basic Tools --> Generic Tools --> Shell`
	:Default Hotkey: < None >

.. image:: /images/Shell.gif
	:align: center

.. note::
	Rationale behind using < K > key: Carried from Silo.

*********************************************************************
Loop Tidy Mid Position <G>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Edge
	:Menu:           :menuselection:`Geometry --> Loop Tidy --> Mid Position`
	:Default Hotkey: < None >

Loop Tidy Mid Position is an indispensable tool for averaging space between loops right after you added some edge loops.
 
.. image:: /images/Loop-Tidy-Mid-Position.gif
	:align: center

.. note::
	Rationale behind using < G > key: I use this quite heavily so.. I did try to see < L > if it works, but it doesn't feel right, so I switch it back to < G >.

*********************************************************************
Loop Relax <Alt+G>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Edge
	:Menu:           :menuselection:`Geometry --> Loop Relax`
	:Default Hotkey: < None >

Many few years back I watched a Gnomon video tutorial by Sze Jones (Digital Female Character Design) to learn more about character modeling, she was using 3ds max and there was this tool she used frequently after adding edge loops to keep the roundness of form. I was really surprised to learn something like this exist and extremely frustrated when it wasn't available in Silo and Maya (Maya now have this I think). I kept searching and looking around for solutions because I need this badly. This is a godsend while working on high poly character. Then I found out about Nvil, and was pretty stoked to find that Nvil already has this within its toolset (I soon switch to Nvil, partly because of this tool.)

.. admonition:: Reference
	:class: refbox

	:Menu:      :menuselection:`View --> Navigation --> Zoom`

.. image:: /images/Loop-Relax.gif
	:align: center

.. note::
	Rationale behind using < Alt+G > key: To make it part of the Loop Tidy/Relax set.

*********************************************************************
Loop Tidy Standard <Ctrl+L>
*********************************************************************

.. admonition:: Reference
	:class: refbox

	:Mode:           Edge
	:Menu:           :menuselection:`Geometry --> Loop Tidy --> Standard`
	:Default Hotkey: < None >

Steve have explained this tool very well on `Nvil's forum <http://samardac.com/nvil-forum//index.php?topic=1170.0>`_

.. image:: /images/Loop-Tidy-Standard.jpg
	:align: center

.. note::
	Rationale behind using < Ctrl+L > key: To make it part of the Loop Tidy/Relax set.
