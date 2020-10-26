# Mask2OBB
### Instanse Segmentation Operations: Convert instance mask to oriented bounding box

<img src = "https://img-blog.csdnimg.cn/20201026111431526.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxNTYyNDQ1,size_16,color_FFFFFF,t_70#pic_center" width="500">

Pipeline of acquiring orientation from annotation. (a)→(b), obtain the contour of the ship from annotation through direct import or transformation. (b)→(c), get the smallest convex envelop according to the contour points. (c)→(d), obtain oriented bounding box from the convex hull points by the rotating calipers method.

### Requirements
```bash
pip install Shapely, numpy, math
```
### Test
```
python mask2obb.py
```
