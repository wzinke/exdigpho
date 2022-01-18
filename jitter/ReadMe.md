# Image Jitter

Inspired by the photographic technique of [Pep  Ventosa](https://www.pepventosa.com) I wanted to generated similar images based on open source tools. This initial script takes one example image and crops it in a different way prior to averaging all cropped images.

Note, these example need to have `../tools` added to the path.

## Example 1: Trees in Snow

|![Trees in Snow](../example_photos/DSC_0099.png)|
|----|
|**Fig. 1:** Original image|

```bash
xmpl_img1="../example_photos/DSC_0099.png"

./mk_jitter $xmpl_img1  -o SnowTree.png
```
The resulting image looks with some white balance adjustment like this:

|![Trees in Snow](SnowTree.png)|
|----|
|**Fig. 2:** Original image|

## Example 1: Magdeburg Buckau

|![Trees in Snow](../example_photos/DSC_2230.png)|
|----|
|**Fig. 3:** Original image|


```bash
xmpl_img2="../example_photos/DSC_2230.png"

./mk_jitter $xmpl_img2 -n 50 -typ screen -Py 15 -Px 25 -o MD_Buckau.png
```
The resulting image looks like this:

|![Magdeburg Buckau](MD_Buckau.png)|
|----|
|**Fig. 4:** Original image|
