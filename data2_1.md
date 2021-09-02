---
follows: volvis
---

### Visualization 4

{(aim|}
This visualization aims to provide the structural demarkation of various fish body elements such as stronger scales on the front part of the fish, gills, fins, it's spinal column and the smoother skin structure. It provides insight into the structural elements and the anatomy of the fish. The structure is identified to be a bony fish which possess a stronger spinal column and the components such as stomach and the swim bladder of the fish could be positionally identified. The bone structure is further explored to understand the rays which are lightweight but strong. 
{|aim)}

{(vistype|}
Demarkation of external and spinal structures of the fish:
![fish0](fish0.png)
Attention on bone structure:
![fish1](fish1.png)
Attachment of the muscular tissue to the central skeleton:
![fish2](fish2.png)
Complete skeleton of the fish:
![fish3](fish3.png)
A sliced view of the fish skeleton:
![fish4](fish4.png)
{|vistype)}

{(vismapping|}
```
Body Structure:
    Data extent: 
        x: 0 to 255
        y: 0 to 255
        z: 0 to 511
    Representation: Volume
    Cell Points:Imagefile
    Blend mode: Composite
    Scaling mode: All exact
    Ray Tracing: Enabled, backend: OSPRay raycaster
    Color preset: Blue-Green-Orange

    Side view: Representation of Gaussian points on the skeleton is applied
    Top view: Representation is set to volume

Attachment of muscular tissue to the bone:
    Color preset: Blue-Green-Orange

Bone Structure and slice:
    Color preset: erdc_magneta
```
{|vismapping)}

{(dataprep|}
The contour filter is applied to extract the skeletal structure of the bone. The volume data is also clipped to show the attachment of the tissue to the bone, it also uses slice filter to show the sliced image of the skeleton.
{|dataprep)}

{(limitations|}
The image focuses on the external and high density features, it does not take into account the muscular tissue that is connected to the central skeleton. The smoother muscle tissue is not explored, it also does not show the internal anatomy of the fish except for the lightweight backbone. The scales of the fish could be explored to understand how the scales are attached to the outer layer of the fish on the fins, the tail part of the fish which plays an important rule in the movement of the fish could be analysed, bony fish possess a swim bladder which helps in balancing the depth of the fish movement which could be explored by slicing the fish at the appropriate position to understand the cross-section of the swim bladder and the underlying organs.
{|limitations)}
