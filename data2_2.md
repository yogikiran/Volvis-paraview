---
follows: volvis
---

### Visualization 5

{(aim|}
The visualization to answer "What's inside a fish"?. The visualization tries to provide different cross-sectional views to identify what is within the fish. It focuses on clipped data to understand the sectional characteristics of the fish anatomy. It also shows the distribution of different structures of a fish within the body of fish. The gradual transition of different fish components can be seen, it also shows the density changes of the skeletal structure.
{|aim)}

{(vistype|}
Focused clipped volume data within the fish:
![fish5](fish5.png)
Sliced skeletal structure and clipped fish volume(clipped across z and y axis):
![fish6](fish6.png)
Clipped fish along the z-axis:
![fish7](fish7.png)
Clipped fish along the z-axis rotated:
![fish8](fish8.png)
Clipped fish along the x-axis:
![fish9](fish9.png)
Clipped fish along the y-axis:
![fish10](fish10.png)
Clipped fish along the y-axis rotated:
![fish11](fish11.png)
{|vistype)}

{(vismapping|}
```
Data Extent unclipped:
    x: 0 to 255
    y: 0 to 255
    z: 0 to 511

Data Extent clipped in corresponding-axes:
    x: 0 to 200 - for the clipped fish along the x-axis
    y: 0 to 200 - for the clipped fish along the y-axis
    z: 0 to 300 - for the clipped fish along the z-axis

Representation: Volume
Color preset: Linear green
Sliced Skeleton Color preset: erdc_magneta
Scaling mode: All approximate
Blend mode: Composite
```
{|vismapping)}

{(dataprep|}
The data is clipped to represent the required volume of cross-sectional volume data. The slice of the data is carried out which is also placed on overlapping extracted subset of a fish. The sub-volume extract is carried out to view the insides of the fish.
{|dataprep)}

{(limitations|}
The visualization tries to find out the objects within the fish with a general structural and cross-sectional overview. It does not convey additional properties or the skeletal structure of the fish, it does not highlight parts such as fins, gill or the head. Since the focus is on identifying objects within the fish if any and not primarly focused on structure understanding, it lacks in demonstrating structural complexities and shows the open volume areas which is free of any foreign objects within it. The visualization can be improved with additional color mapping to focus on the external contours and the internal organ structures.
{|limitations)}
