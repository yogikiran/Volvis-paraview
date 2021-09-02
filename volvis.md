---
elm:
  dependencies:
    gicentre/elm-vegalite: latest

narrative-schemas:
  - volvis
---

## Author: Yogi Kiran Jayaramu

The Volume rendering techniques are employed to demonstrate and visualize the Mystery Datasets. One example from the Paraview is also visualized to obtain insights of the object, the object used is a human head which is available to download or explore in the official Paraview website:
:<https://www.paraview.org/download/>.

### Visualization 1

The example file - 'headsq' which has a volumetric data provides the scalar volumetric data unlike the image files in the mystery dataset. This example has a cylindrical boundary and a cropped human head with an object in his/her oesophagal tract(looks similar to a endotracheal tube) and on the external it is suspended outside the mouth of the human head.

{(aim|}
The Visualization helps in identifying the basic structure of a human head by thresholding the required scalar values (removing the external cylinder) and also to understand the complex interior structure of human head anatomy and the modelling of human tissue that is attached to the skull of a human head. It also provides the information of high scalar point distributions which is shown using a color mapping and shade blend. The structural complexity of the skull and the sliced data information portraying low density areas and tubular spaces in the human head is also interpreted with the cross-sectional data that is obtained from the Volume visualization.
{|aim)}

{(vistype|}
Thresholding to extract human head from the cylinder and portraying different angles of the human head with the appropriate color mapping:
![head1](head1.png)
Contour volumetric data extracted and visualized in different angles:
![head2](head2.png)
High Density scalars represented with the color map:
![head3](head3.png)
Sliced view showing the top view of the human skull along with the surrounding attached tissue:
![head4](head4.png)
Sliced view showing Nasal, Oesophagal tracts and the section of the spinal column:
![head5](head5.png)
{|vistype)}

{(vismapping|}
```

Cell points: Scalars


Thresholded image:
  Representation: Volume
  Opacity: Enabled and linear mapping
  Color preset: Viridis
  Color Space: Linear

Contour Volumetric Data:
  Representation: Surface
  Color preset: Gray and red - default
  Contour by: Scalars
  value range: single value - 2047.5
  Opacity value: 1
  Scaling mode: All exact
  Compute Normals
  Generate Triangles

High Density Scalars:
  Color preset: Jet
  Color Discretize: Number of table values - 256

Sliced views:
  Color preset: Black, Blue and White
  Contour: Enabled for slice
```
{|vismapping)}

{(dataprep|}
The Head volume data is obtained by thresholding and removing the cylindrical layer around the human head, contour filter is further applied to obtain the skeletal structure of the human head which shows the spinal column and the facial bone structure. Slicing is also carried out to obtain the cross-sectional data.
{|dataprep)}

{(limitations|}
The visualization focused majorly on denser and skeletal figures and did not capture the tissue complexity except for the simple model showing the attachment areas(highlighted in yellow in the thresholded image). The visualization does not delve deeper to explore the nerval tissues and the cross-sectional analysis. It is not physically realistic and does not capture the complex internal details or the complex anatomy of the human head. The given volume data can also be further explored using clipped data by extracting subsets and exploring focus areas such as the eye, nose, etc,.
{|limitations)}

