---
follows: volvis
---

### Visualization 2

{(aim|}
The visualization to answer "What's inside a teddy bear?". The visualization majorly cleans on the provided volumetric imagefile data to identify the mystery object and to also look inside the teddy bear once it is identified. The teddy bear clipping is carried out to identify the objects within the teddy bear. Apart from the contour data, the distribution points and the stitch points of the teddy bear is visualized to understand the construction of the teddy bear in reality.
{|aim)}

{(vistype|}
Ray traced extracted data:
![teddy1](teddy1.png)
Contour and volume focused stitch-identified teddy bear:
![teddy2](teddy2.png)
Transformed teddy bear to clearly visualize teddy bear:
![teddy3](teddy3.png)
clipped teddy bear to look what's insdie:
![teddy4](teddy4.png)
{|vistype)}

{(vismapping|}
```
Cell points: Imagefile
Data Extent:
    x-axis: 0 to 511
    y-axis: 0 to 511
    z-axis: 0 to 62
Representation: Volume and contour overlapped
Scaling mode: All exact
Volume Rendering mode: smart
Blend mode: Composite
Color preset: Green-white linear
Volume of Interest - V OI(Extracted subset data extent):
    x-axis: 40 to 430
    y-axis: 50 to 430
    z-axis: 0 to 62
Transform function values:
    z value - scaled factor:
        x-axis: 0
        y-axis: 0
        z-axis: 6

Ray traced data:
    backend: OSPRay raycaster
```
{|vismapping)}

{(dataprep|}
The teddy bear is cleaned by color mapping transfer function, Extract subset filter is applied to obtain the subset of the teddy bear object. The transform function is applied to z transform the teddy bear to improve the visualization, the teddy bear is then clipped along both y and x axis diagonally which will help in visualizing the insides of teddy bear.
{|dataprep)}

{(limitations|}
The visualization aims only to look inside the teddy bear, the transform function adds additional scaled data which will make the visualization pleasant but does not add any value to identify the objects within it. The teddy bear is clipped diagonally to identify if there are any objects, it vaguely provides information regarding the type of material and fails to show the inner fur material clearly. The visualization is not clipped multiple times or at multiple sections to look thoroughly inside the teddy bear, although the diagonal clip shows the majority insides of a teddy bear, it doesn't ensure the complete search within the teddy bear.
{|limitations)}
