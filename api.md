# API

Some 3d concepts are prerequisite. The related links will be attached in the followings.

---

This framework is using [perspective projection](https://en.wikipedia.org/wiki/3D_projection) to map three-dimensional points into the two-dimensional graph. In `perspective projection`, we need to locate the **sight point** (equivalent to a camera) . Any sight point can be specified with four elements: `anchor`, `d`, `alpha`, `beta`. 

```
.setCamera(opt)
```

property|type|description|required|default
:-:| :-: | :-: |:-: | :-: 
anchor|Array|the camera always needs a focused point|false|[0, 0, 0]
d| Number| the distance between the camera and the anchor| false| 300
alpha| Number| image that the camera is rotating around the anchor. The track can be described as rotating `alpha` horizontally and `beta` vertically| false| 0
beta| Number| image that the camera is rotating around the anchor. The track can be described as rotating `alpha` horizontally and `beta` vertically| false| 0

---

In `perspective projection`, there is also a screen. 

```
.setCamera(opt)
```

---

clean the graph and reset all setting options. 

```
.reset()
```

---