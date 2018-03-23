# Camera Lens Smear Detection- OpenCV and Python

This application helps to detect any kind of small smears on camera lens.
This application is useful in Street Map designing.

Flowchart for Algorithm procedure. 


```flow
st=>start: Input Images
op=>operation: Convert all images to same size (width & height)
op=>operation: Calculate mean of all images
op=>operation: Convert to grayscale and use Threshold image using openCV
cond=>condition: is Mask satisfy min-max smear category?
op=>operation: apply mask to the images.
e=>end: Final Result

st->op->cond
cond(yes)->op
cond(no)->e
```