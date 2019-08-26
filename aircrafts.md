# Aircraft Tagging 
> Version 2019-08-26

## Geometry

Planes in the imagery should be identified with 5-points polygons. For planes, polygons should be drawn with the following method:

- Point 1 = aircraft nose
- Point 2 = right wing
- Point 3 and 4 = tail
- Point 4 or 5 = left wing

![Aircraft 5 points](http://imagery.airbusds-geo.com/examples/aircraft01.png)

For helicopters, the five points should be as follows:

- Point 1 = tail 
- Point 2, 3, 4, 5 = end of each blade

![Helicopter 5 points](http://imagery.airbusds-geo.com/examples/aircraft02.png) 

In some cases, you might need to use more than 5 points. *The main objective is to make sure that the polygon encompass the whole aircraft*.

## Classes

The aircraft should be classified in 4 categories:

- **small_aircraft** : light aircrafts, private jets
- **large_commercial** : passenger aircraft

![Large Commercial](http://imagery.airbusds-geo.com/examples/large_commercial_01.png)

- **helicopter** : all types including military, non-militayr, simple or double rotors

![Helicopter](http://imagery.airbusds-geo.com/examples/helicopter_01.png)

![Helicopter](http://imagery.airbusds-geo.com/examples/helicopter_02.png)

- **fighters** : combat aircrafts, military fighters, military jets

![Fighters](http://imagery.airbusds-geo.com/examples/fighter_01.png)

![Fighters](http://imagery.airbusds-geo.com/examples/fighter_02.png)

- **bombers** : military bombers. They typically have large wingspan, four reactors, thin bulk

![Bombers](http://imagery.airbusds-geo.com/examples/bombers_01.png)

![Bombers](http://imagery.airbusds-geo.com/examples/bombers_02.png)

- **other_large_military** : all other large military planes like military transport planes and AWACS. They typically have large bulk to carry tanks or other military equipment.

![Large Military](http://imagery.airbusds-geo.com/examples/other_large_military_01.png)

## Notes

The length or wingspan of the combat aircrafts and helicopters should be larger **15 pixels**. If you encounter objects on the tarmac that might be aircrafts, please tag them as **small_aircraft**.
