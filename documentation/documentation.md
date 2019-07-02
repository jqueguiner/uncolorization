Image Uncolorization will vintage your picture to turn them into black and white style.


Read this paper to learn more about this technic:
[Color-to-Grayscale: Does the Method Matter in Image
Recognition?](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0029740&type=printable)

```
@article{10.1371/journal.pone.0029740,
    author = {Kanan, Christopher AND Cottrell, Garrison W.},
    journal = {PLOS ONE},
    publisher = {Public Library of Science},
    title = {Color-to-Grayscale: Does the Method Matter in Image Recognition?},
    year = {2012},
    month = {01},
    volume = {7},
    url = {https://doi.org/10.1371/journal.pone.0029740},
    pages = {1-7},
    abstract = {In image recognition it is often assumed the method used to convert color images to grayscale has little impact on recognition performance. We compare thirteen different grayscale algorithms with four types of image descriptors and demonstrate that this assumption is wrong: not all color-to-grayscale algorithms work equally well, even when using descriptors that are robust to changes in illumination. These methods are tested using a modern descriptor-based image recognition framework, on face, object, and texture datasets, with relatively few training instances. We identify a simple method that generally works best for face and object recognition, and two that work well for recognizing textures.},
    number = {1},
    doi = {10.1371/journal.pone.0029740}
}
```

- - -

EXAMPLE  
![output](https://i.ibb.co/5Y0M2Xb/example.png)

- - -
INPUT

``` json
{
  "url": "https://i.ibb.co/x3srpR0/input.jpg"
}
```
- - -
EXECUTION
```bash
curl -X POST "https://MY_SUPER_IP:5000/image-uncolorization/process" -H "accept: image/png" -H "X-OVH-Api-Key: XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX" -H "Content-Type: application/json" -d "{\"url\":\"https://i.ibb.co/x3srpR0/input.jpg\"}"
```
- - -
OUTPUT
Binary output png image.
![output](https://i.ibb.co/LnqSVRv/output.jpg)


