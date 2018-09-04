###############################
Transformations
###############################


.. image:: /images/Transformations-list.jpg
	:align: center

********************
Toggle Snapping <U>
********************

I use a hotkey <U> to toggle snapping and then use the usertools window buttons to select snappings of different types (vertex, edge, edge midpoint, face, face midpoint).

::

	Manipulation > Snapping Options > Snapping Enabled

.. image:: /images/Snapping.gif
	:align: center

Nvil's default snapping UI is utilizing a dropdown menu. I find that only one of them can be turn on at a time. It is also not easy to glance at their status (there is Show Snapping State in Heads Up display but icons should be more readable than text I guess).

.. image:: /images/Nvil-default-snapping-ui.jpg
	:align: center

.. note::
	Rationale behind using <U> key: It's shaped like a Magnet :)

.. note::
	Default Nvil hotkey for this: <Ctrl+X1>. (Not sure what X1 is and how to trigger it...)

******************************
Axis Move/Rotate/Scale <W/E/R>
******************************

Axis Move/Rotate/Scale are a set of streamline tools that I played with recently. While learning Blender, I grown fond of its Grab/Rotate/Scale combo with x/y/z, for example <G> followed by <X> will translate selected object in X Axis. You can also specify the value of how much you want to transform, which is quite handy when rotating, for example <R>, <Z>, <9>, <0> will rotate selected object by 90 degree in Z. I am pretty stoked when I found Nvil also has this option, albeit Blender's one still has a better feel to it.

.. image:: /images/Axis-Move-and-Scale.gif
	:align: center


Setup for streamline tool (All modes):

.. image:: /images/Axis-Move-setup.jpg

.. note::
	Rationale behind using <W/E/R> key: Commonly used in 3d applications (except Blender).

*******************
Local Move <Ctrl+W>
*******************

A streamline tool that combines 3 different variation of local/normal move. The first one Tweak_NormalMove(IgnorePolygonNormal) works similarly to Maya's Transform Component. The selected subojects will be translated outwards according to each vertices normal. The second Local Move Selection will get a normal out of each suboject island (I guess that's how it works) and move them according to that normal (instead of each vertices normals). The Last one Polygon_LocalMove_PolygonNormal works similar to the second one but it only works on Polygon (Face) selection, but it's not just the subobject mode, I also find them behaves a bit differently.

In a situation where you find one not working as desired, you can try the other two and see which one works the best.

.. image:: /images/Local-Move.gif
	:align: center

Note that in the gif I was using <LMB> the first time and <MMB> the second time. I didn't show the use of <RMB> because it would behaves just like <MMB> in this case.

Setup for streamline tool (subojects mode):

.. image:: /images/Local-Move-setup.jpg

.. note::
	Rationale behind using <Ctrl+W> key: 'W' as used in Move. Why not <Alt+W>? Because I am using <Alt+W> for a more frequently used Vertex Weld.

.. note::
	Default Nvil hotkey for this: Nvil actually has a built-in tool for this and it's called Local Move Polygon, hotkey is <H>. It is composed of Polygon_LocalMove_PolygonNormal, Polygon_LocalMove_CursorDirection and Polygon_LocalMove_AverageNormal. I moved Polygon_LocalMove_PolygonNormal to RMB and replace the others with my preferred tools.

********************
Local Scale <Ctrl+R>
********************

Sometimes what you want is just scale those polygons in their place. This is a 

.. image:: /images/Local-Scale.gif
	:align: center

Setup for streamline tool (subojects mode):

.. image:: /images/Local-Scale-setup.jpg

.. note::
	Rationale behind using <Ctrl+R> key: 'R' as used in Scale.

.. note::
	Default Nvil hotkey for this: Nvil actually has a built-in tool for this and it's called Misc Subobject Tools, hotkey is <N>. It is composed of Local Rotate Selection <LMB> and Local Scale Selection <RMB>.

******************
Snap Selection <.>
******************

Snap Selection is a streamline tool that comes with Nvil's Built-in Tools. It is composed of Snap_Position_Only, Differential_Snap and Snap_Position_Normal. In the gif below, I am using just the third RMB option to snap some primitives to the cloth.

.. image:: /images/Snap_Selection.gif
	:align: center

Setup for streamline tool (Nvil Default):

.. image:: /images/Snap-Selection-setup.jpg

.. note::
	Rationale behind using <.> key: Hmm... because I don't use it too much so I decide to put it somewhere on the right hand side and out of those keys, some were already used for other purposes and '.' got chosen because maybe the key also has a '>' symbol that looks like the movement of snap? It doesn't really matter I guess..

.. note::
	Default Nvil hotkey for this: <None>
