# Aircraft Tagging

> Version 2019-09-30

## Geometry

Planes in the imagery should be identified with 5-points polygons. For planes, polygons should be drawn with the following method:

- Point 1 = aircraft nose
- Point 2 = right wing
- Point 3 and 4 = tail
- Point 4 or 5 = left wing

![Aircraft 5 points](resources/aircraft/aircraft01.png)

For helicopters, the five points should be as follows:

- Point 1 = tail
- Point 2, 3, 4, 5 = end of each blade

![Helicopter 5 points](resources/aircraft/aircraft02.png)

In some cases, you might need to use more than 5 points. **The main objective is to make sure that the polygon encompass the whole aircraft**.

## Classes

The aircraft should be classified into the following 6 categories:

- **small_aircraft** : light aircrafts for leisure, private jets and small passengers aircrafts. Most of these aircrafts have propellers or maximum two small reactors. In that case, the engines are mounted on the fuselage or body of the plane. They typically accomodate 2 to 20 persons maximum. This category also includes gliders. 

![Small Aircrafts](resources/aircraft/small_aircraft_01.png)
![Small Aircrafts](resources/aircraft/small_aircraft_02.png)
![Small Aircrafts](resources/aircraft/small_aircraft_03.png)

- **large_commercial** : large aircrafts from commercial companies carrying passenger or fret. These aircrafts generally have 2 to 4 engines mounted under the wings. Main manufacturers are Airbus and Boeing. Most common commercial aircrafts are manufactured by Airbus (A320, A340, A380) and Boeing (B737, B747, B777). They mostly have two or four reactors but some have three (McDonnell Douglas DC-10). Lighter commercial aircrafts from ATR, Bombardier or Embraer also fall in this category.

![Large Commercial](resources/aircraft/large_commercial_01.png)
![Large Commercial](resources/aircraft/large_commercial_02.png)

- **helicopter** : all types including military, non-militayr, simple or double rotors

![Helicopter](resources/aircraft/helicopter_01.png)
![Helicopter](resources/aircraft/helicopter_02.png)

- **fighters** : combat aircrafts, military fighters, military jets

![Fighters](resources/aircraft/fighter_01.png)
![Fighters](resources/aircraft/fighter_02.png)

- **bombers** : military bombers. They typically have large wingspan, four reactors, thin bulk

![Bombers](resources/aircraft/bombers_01.png)
![Bombers](resources/aircraft/bombers_02.png)

- **other_large_military** : all other large military planes like military transport planes and AWACS. They typically have large fuselage to carry tanks or other military equipment. Their shapes are very similar to these of commercial aircrafts. AWACS are easy to identify thanks to the circular radar above them.

![Large Military](resources/aircraft/other_large_military_01.png)
![Large Military](resources/aircraft/other_large_military_02.png)

## Important notes

The length and wingspan of aircrafts and helicopters should be **larger than 10 pixels**.

If you encounter objects on the tarmac that might be aircrafts but do not fall in the previous categories, please tag them as **unknown_aircraft**.

**Discard** any aircraft that is truncated at the border of the imagery. **Do not discard** an aircraft that is not fully visible for other reasons (i.e. partially covered by a shed).

**Do not annotate** blimps (a.k.a zeppelin), hot air balloons, dismantled aircrafts or aircrafts pieces such as an helicopter without blades, an aircraft without wings or wings alone.

![Not aircraft](resources/aircraft/not_aircraft.png)
![Not helicopter](resources/aircraft/not_helicopter.png)

**Annotate all aircrafts** including flying aircrafts i.e. not resting on the taxiways. You may notice a chromatic halo close to a flying aircraft as below.

![Flying aircraft](resources/aircraft/flying_aircraft.png)
