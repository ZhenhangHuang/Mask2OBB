# Mask2OBB
### Instanse Segmentation Operations: Convert instance mask to oriented bounding box

<img src = "https://img-blog.csdnimg.cn/20201026111431526.jpg?x-oss-process=image">

Pipeline of acquiring orientation from annotation. 
(a)→(b), obtain the contour of the instance from annotation through direct import or transformation. 
(b)→(c), get the smallest convex envelop according to the contour points.
(c)→(d), obtain oriented bounding box from the convex hull points by the rotating calipers method.

### Requirements
```bash
pip install Shapely, numpy
```
### Test
```
python mask2obb.py
```
