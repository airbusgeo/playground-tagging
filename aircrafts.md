# Aircraft Tagging

> Version 2020-10-12

## Geometry

Planes in the imagery should be identified with 5-points polygons. 

### For planes, polygons should be drawn with the following method:

- Point 1 = aircraft nose
- Point 2 = right wing
- Point 3 and 4 = tail
- Point 4 or 5 = left wing

  ![Aircraft 5 points](resources/aircraft/aircraft01.png)

### For helicopters, the five points should be as follows:

- Point 1 = tail
- Point 2, 3, 4, 5 = end of each blade

  ![Helicopter 5 points](resources/aircraft/aircraft02.png)

In some cases, you might need to use more than 5 points. **The main objective is to make sure that the polygon encompass the whole aircraft**.

## Classes

We focus into **detection** of the aircraft and **reconnaissance** of its general type. As such, the aircraft should be classified into the following 6 main categories and potential sub-categories:

- **`small_aircraft`**

  Light aircrafts for leisure, private jets and small passengers aircrafts.  

  This category can have the following sub-categories:

  - **`leisure_aircraft`**

    Aircrafts used for leisure activiy. Most of these aircrafts have propellers. Their length is maximum of 12 m. i.e. 25 pixels on 50cm imagery. This category also includes gliders which have a much larger wingspan.

    ![Small Aircraft](resources/aircraft/small_aircraft_01.png)
    ![Small Aircraft](resources/aircraft/small_aircraft_03.png)

  - **`private_jet`**

    This category of small aircrfats has usually maximum two small reactors. In that case, the engines are mounted on the fuselage or body of the plane. They can acommodate up to 16 persons. Their length is between 12 m. and 25 m. i.e. 25 to 50 pixels on 50cm imagery. More information on [Wikipedia](https://en.wikipedia.org/wiki/Business_jet).

    ![Small Aircraft](resources/aircraft/small_aircraft_02.png)

  - **`regional_commercial`**

    Lighter commercial aircrafts from ATR, Bombardier or Embraer fall in this category. They typically accomodate up to 100 persons maximum. Their length is between 25 m. and 40 m. i.e. 50 to 80 pixels on 50cm imagery. More information on [regional airliners](https://en.wikipedia.org/wiki/List_of_regional_airliners).

    ![Regional Commercial](resources/aircraft/large_commercial_02.png)

- **`large_commercial`**

  Large aircrafts from commercial companies carrying more than 100 passengers or cargo. These aircrafts have a lenght of 40 m. and more (i.e. over 80 pixels on 50cm imagery). Most common commercial aircrafts are manufactured by Airbus (A320, A340, A380) and Boeing (B737, B747, B777). They mostly have two or four reactors mounted under the wings but some have a third reactor on the tail (McDonnell Douglas DC-10). More information on [airliners](https://en.wikipedia.org/wiki/Airliner).

  ![Large Commercial](resources/aircraft/large_commercial_01.png)
  

- **`helicopter`**

  This sub-class includes all helicopters, civilian and military, with single and double rotors. Military helicopters, as civilian ones, are mostly used for transport, observation and rescue but can also be attack helicopters. More information on [helicopters](https://en.wikipedia.org/wiki/Helicopter) and [military helicopters](https://en.wikipedia.org/wiki/Military_helicopter).

  ![Helicopter](resources/aircraft/helicopter_01.png)
  ![Helicopter](resources/aircraft/helicopter_02.png)

- **`fighters`**
  
  This sub-class includes combat aircrafts, military fighters and military jets

  ![Fighters](resources/aircraft/fighter_01.png)
  ![Fighters](resources/aircraft/fighter_02.png)

- **`bombers`**
  
  This sub-class is for military bombers. They typically have large wingspan, four reactors, thin bulk

  ![Bombers](resources/aircraft/bombers_01.png)
  ![Bombers](resources/aircraft/bombers_02.png)

- **`other_large_military`**

  All other large military aircrafts all in this sub-class. They are mainly military transport planes, refuelers and AWACS. They typically have large fuselage to carry tanks or other military equipment. Their shapes are very similar to these of commercial aircrafts. AWACS are easy to identify thanks to the circular radar above them.

  ![Large Military](resources/aircraft/other_large_military_01.png)
  ![Large Military](resources/aircraft/other_large_military_02.png)

## Important notes

The length and wingspan of aircrafts and helicopters should be **larger than 10 pixels**.

If you encounter objects on the tarmac that might be aircrafts but do not fall in the previous categories, please tag them as **unknown_aircraft**.

**Do not annotate** any aircraft that is truncated at the border of the imagery. This should be covered by appropriate overlapping of imagery tiles. 

**Annotate** an aircraft that is not fully visible for other reasons (i.e. partially covered by a shed).

**Do not annotate** blimps (a.k.a zeppelin), hot air balloons, dismantled aircrafts or aircrafts pieces such as an helicopter without blades, an aircraft without wings or wings alone.

![Not aircraft](resources/aircraft/not_aircraft.png)
![Not helicopter](resources/aircraft/not_helicopter.png)

**Annotate all aircrafts** including flying aircrafts i.e. not resting on the taxiways. You may notice a chromatic halo close to a flying aircraft as below.

![Flying aircraft](resources/aircraft/flying_aircraft.png)
