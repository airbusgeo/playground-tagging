# Vehicles Tagging

> Version 2019-11-06

## Geometry

This project aims to tag **road vehicles**.

Records should be annotated as **oriented bounding-box** (i.e. a rectangle or **4-vertices polygon**, with no differentiation between the front and the back of a car).

## Classes

Every record must have a class attribute of either **car** or **truck**. No records should ever comprise more than one object.

- **Car**

![Cars](resources/vehicles/cars01.png)

This class includes utility vehicles (i.e. pickup, van)

![Pickup](resources/vehicles/pickup01.png) ![Van](resources/vehicles/van01.png)

- **Truck**

This class includes generic trucks:

![Generic Truck](resources/vehicles/generic_truck01.png) ![Generic Truck](resources/vehicles/generic_truck02.png)

trailer trucks:

![Generic Truck](resources/vehicles/trailer_truck01.png) ![Generic Truck](resources/vehicles/trailer_truck02.png)

and buses:

![Bus](resources/vehicles/bus01.png) ![Bus](resources/vehicles/bus02.png)
