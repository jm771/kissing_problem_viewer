# kissing_problem_viewer
AlphaEvolve has found an improved solution to the kissing problem in 11 dimensions. (How many N-Balls can you put adjacent to an N-Ball without intersection). Matt Parker reported on this here: https://www.youtube.com/watch?v=sGCmu7YKgPA
Neither Google not Matt had a visualization for this - so I threw one together here.

Basically, we define a view plane, and provide 10 sliders for rotating that view plane. Then we orthographically map each Ball center onto the view plane. We draw a cicle at each of these mapped centers. Plus we draw a red circle at the origin for the N-ball being kissed. To try and get some sense of depth, we define a camera view point which is also rotated by the sliders, and circles are scaled in inverse proportion to their distance to the view point.
