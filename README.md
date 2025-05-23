# kissing_problem_viewer
AlphaEvolve has found an higher lower bound to the kissing number in 11 dimensions. (How many N-Balls can you put adjacent to an N-Ball without intersection). Matt Parker reported on this here: https://www.youtube.com/watch?v=sGCmu7YKgPA
Neither Google not Matt had a visualization for this - so I threw one together here.

Basically, we define a view plane, and we orthographically map each ball center onto the view plane. We draw a cicle at each of these mapped centers. Plus we draw a red circle at the origin for the N-ball being kissed. To try and get some sense of depth, we offset the view plane from the origin, and circles are scaled in inverse proportion to their distance from the view plane. This can be turned off via the "Scale circles by distance" control to get a true orthographic projection.

### Control info
#### Dimensions
I have also included the optimal kissing number solutions in 3 and 4 dimensions - which should help build some intuition for what the controls do. Start with them before moving to 11D

#### Rotation controls
We maintain a basis for the view. The X and Y axis of the view plane are the first two dimensions of this basis. The view plane is offset from the origin in the third dimension. Clicking the X-3 (+) button rotates the basis so as to rotate the X axis slightly towards the positive axis for dimension 3 (in the current basis). There is no need to have buttons for X-1 and Y-2 as you cant move an axis towards itself. The "Rotate in plane" button controls the special case of rotating between X and Y axes that otherwise would be duplicated. If this description doesn't make sense - try playing with it in 3D and 4D to develop an intuition.

#### Scale circles by distance:
Turn off to have a true orthographic projection with all circles to scale. When turned on, balls closer to the view plane than the origin are scaled up, and balls further from the view plane then the origin are scaled down to create some sense of depth. (the red ball at the origin is always unchanged).

#### Zoom 
Effectively zooms in and out of the image once it's been collapsed to 2D

#### Circle Radius
The default setting of 0.5 with "scale circles by distance" turned off shows the cicles "to scale". You'll note the circles overlap. That's because we're only viewing two of the dimensions. Have a play with the 3d case to convince yourself despite the 3D balls not overlapping, when you view a 2D projection their outlines do overlap. 

In 11D the overlapping is very noisy and it might be easier to reduce the circle size significantly and view the circles as the center of the kissing balls, rather than the balls themselves.

#### Rotation Step size
The size of rotation made by the +/- buttons in radians
