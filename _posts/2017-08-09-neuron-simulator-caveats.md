---
layout: post
title:  "Neuron Simulator Caveats"
date:   2017-08-09 17:40:32 +0300
categories: NeuronSimulator
---

- The best method to describe sections:
  ```
  sectionname1 {
    stmt1
    sectionname2 {
  ```
- `soma.v(0.5)` will return the value of the segment that contains the 0.5 point of normalized length of `soma`.
- Segmenting. `nseg` should be odd so when you play with discretization the middle segment always stays middle. The best option to discretize is to scale by 3 and see how the new discretization is better than the previous one. The even scale will change the middle segment position, so don't use it.
- Attach sections at 0 or 1 for accuracy. Attaching to any other place would attach to some internal segment that depends on `nseg`.
- Don't set diameter to zero. With stylized declaration we can check
  ```
  forall for (x) if (diam(x)<1) { print secname(), " ", x, " ", diam(x) }
  ```
  With 3-D declaration
  ```
  forall for i=0,n3d()-1 if (diam3d(i)==0) { print secname(), " ", i }
  ```
- When 3-D points exist, they determine the calculation of `L`, `diam`, `area`,`ri` values. So anytime a Shape is created for the stylized definition, the shape changes those values slightly.
- When a point process is no longer referenced by any object reference, it is removed from the section and destroyed.
- Discretization should be based on AC length rather than DC length. Use `d_lambda` variable for that. For more details see the note ["AC vs DC length"](DC_vs_AC_length_constant.md).
- Abrupt diameter changes should be restricted to section boundaries.
- Be careful with the position of a point process when you change `nseg`.
- Range variables should be refreshed after a change of `nseg`.
- Do not write your own Simulation control. Use the Neuron's one. It has lots of hooks to customize. Otherwise it will be crazy to sync them.
- Put `load_file("nrngui.hoc")` in your script in order to load GUI.
- Always set default section because many of the GUI tools, such as voltage graphs, shape plots, and point processes, must
refer to a particular section at the moment they are spawned.
- Barbed wire. Always set geometry on your own because at every branch point, NEURON's internal routine for rendering shapes makes its own decision, by a rule: make a fork with one child pointing to the left and the other to the right by the same amount relative to the orientation of the parent.
- Use relative coordinates when specifying `pt3add`.
- To avoid a disappearing section always connect the 0th end of a child section to its parent. So do `connect dend[1](0), dend[0](1)` instead of `connect dend[0](1), dend[1](0)`.
- Caution when combining GUI tools and hoc statements. Changes you make at the hoc level are not propagated to the GUI tools, so if you then make any changes with the GUI tools, it is likely that all the changes you made with hoc statements will be lost.
