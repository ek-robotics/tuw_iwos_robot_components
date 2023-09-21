# Independent Wheel Offset Steering - Robot Components

This repository contains the [FreeCAD](https://www.freecad.org/) files for the components of the Independent Wheel Offset Steering robot prototype.

This prototype was created by Eugen Kaltenegger as part of the master thesis. Please check out the thesis for details on the Independent Wheel Offset Steering.

## Project Structure

This project contains four folders with robot parts designed in CAD. Each folder holds the FreeCAD file(s) (`<file_name>.FCStd`) as well as the a folder with the `stl` files and a folder with the `step` files for each part of the FreeCAD file(s). All FreeCAD files in this repository are verified to open with FreeCAD version `0.21.1`.

The  `stl` format should is suitable for fabrication. The `step` files should enhance compatibility with other tools then CAD tools.

Additionally a folder with pictures of the robot is placed in this repository.

### Folder Content

- `00_fork`: This folder contains the parts of the fork, the fork mount and the caster. The fork is designed to be operated with a Dynamixel MX-106 and a 4'' wheel (similar to [this](https://de.aliexpress.com/item/32597304241.html?spm=a2g0o.productlist.0.0.577e3e000hS516&algo_pvid=a5219ba5-5575-4274-97ab-7a0253f323d2&algo_expid=a5219ba5-5575-4274-97ab-7a0253f323d2-10&btsid=0b0a556e16173642780354782e8e1a&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)). Between the fork and the fork mount a pivot bearing (such as [this](https://www.amazon.de/gp/product/B088TR2KKZ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)) should be placed.

- `01_electronics`: This folder contains a mount for lead batteries and a case suitable to place all electronics components inside. This includes a mount for the Trinamic TMCM 1640 controller and the Dynamixel U2D2.
- `02_bumper`: This folder contains the bumpers attached to the robot. This are designed to break in case of an high impact collision.
- `03_mount`: This folder contains various mounts:
  - Mount for the Hokuyo Laser Scanner (UTM-30LX-EW)
  - Mount for the NUC Computer and the XTPower battery pack (MP-23000)
  - Mount for the router (GL iNet AC1200 Wireless Travel Router)
  - Mount for the IMU (TransducerM TM352)
  - Mount for the reflective markers for the OptiTrack system

## Printing and Assembly

Slicing and printing the parts has been done with [Prusa Slicer](https://www.prusa3d.com/de/page/prusaslicer_424/) and a [Prusa MK3S+](https://www.prusa3d.com/de/produkt/original-prusa-i3-mk3s-3d-drucker/) using [Prusa PETG](https://www.prusa3d.com/de/kategorie/prusament-petg/). For most of the parts 25 percent infill will be enough.

The assembly should be done with M2, M3 and M4 screws. Many parts require press fit threads. These can be inserted into 3D printed parts with a solder iron. [Solder iron tips](https://www.amazon.de/ruthex-L%C3%B6tspitzen-Einschmelzhilfen-L%C3%B6tkolbenspitzen-Gewindeeins%C3%A4tze/dp/B0CDBSGSXY/ref=sr_1_9?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=1Q6NERTJ8BOR7&keywords=l%C3%B6tkolben%2Bgewinde&qid=1695286817&sprefix=l%C3%B6tkolben%2Bgeinde%2Caps%2C212&sr=8-9&th=1) specially designed for this task can ease this process. 

Note: the fork can be reinforced with wood screws from the bottom. A screw with a length of 6cm should be perfect.

