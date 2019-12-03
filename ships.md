# Ships Tagging

> Version 2019-12-03

## Geometry

This project aims to tag **ships**.

Records should be either annotated as **oriented bounding-box** (i.e. a rectangle or **4-vertices polygon**, with no differentiation between the front and the back of a car) or a **n-points polygon** 

<p align="center"> 
    <img src="resources/ships/geom.png" width="200" height="200" title="Examples of ship geometries">
</p>

## Classes

A taxonomy has been defined in order to represent the different specific cases a user can encounter.

<p align="center"> 
    <img src="resources/ships/taxonomy.png" height="400" title="Ship Detection taxonomy">
</p>

Every record must have either **marina**, **ship** or **unkown** tag. A marina is a dock or basin with moorings and supplies for yachts and small boats. 


<p align="center"> 
    <img src="resources/ships/marina.png" height="200" title="Example of a marina">
    <img src="resources/ships/marina_2.png" height="200" title="Example of a marina">
</p>

The tag **unknow** is used when the user is sure that the object is neither a **ship**, nor a **marina**. This one should not be used very often.

When the user recognise an object as a **ship**, he may be able to go one step further and find the **class** of the vessel. **8** classes have been selected to represent the whole diversity of the ships that may be encountered. A ninth class has been added, **unclassified**, to be used when the user hesitate between several classes for a single object. For smaller ships, the difference between two ships of different classes are extremely minimal, and often, the context of the scene is used to settle the dispute. Please find the different classes that may be encountered with some examples:

- **Barge**

<p align="center"> 
    <img src="resources/ships/barge.png" height="200" title="Example of a barge">
    <img src="resources/ships/barge_2.png" height="200" title="Example of a barge">
    <img src="resources/ships/barge_3.png" height="200" title="Example of a barge">
</p>

- **Fishing vessel**

<p align="center"> 
    <img src="resources/ships/fishing.png" height="200" title="Example of a fishing vessel">
    <img src="resources/ships/fishing_2.png" height="200" title="Example of a fishing vessel">
    <img src="resources/ships/fishing_3.png" height="200" title="Example of a fishing vessel">
</p>

- **Leisure vessel**

<p align="center"> 
    <img src="resources/ships/leisure.png" height="200" title="Example of a leisure vessel">
    <img src="resources/ships/leisure_2.png" height="200" title="Example of a leisure vessel">
    <img src="resources/ships/leisure_3.png" height="200" title="Example of a leisure vessel">
</p>

- **Merchant vessel**

<p align="center"> 
    <img src="resources/ships/merchant.png" height="200" title="Example of a merchant vessel">
    <img src="resources/ships/merchant_2.png" height="200" title="Example of a merchant vessel">
    <img src="resources/ships/merchant_3.png" height="200" title="Example of a merchant vessel">
    <img src="resources/ships/merchant_4.png" height="200" title="Example of a merchant vessel">
</p>

- **Military vessel**

<p align="center"> 
    <img src="resources/ships/military.png" height="200" title="Example of a military vessel">
    <img src="resources/ships/military_2.png" height="200" title="Example of a military vessel">
    <img src="resources/ships/military_3.png" height="200" title="Example of a military vessel">
    <img src="resources/ships/military_4.png" height="200" title="Example of a military vessel">
</p>

- **Passenger vessel**

<p align="center"> 
    <img src="resources/ships/passenger.png" height="200" title="Example of a passenger vessel">
    <img src="resources/ships/passenger_2.png" height="200" title="Example of a passenger vessel">
    <img src="resources/ships/passenger_3.png" height="200" title="Example of a passenger vessel">
</p>

- **Speed vessel**

<p align="center"> 
    <img src="resources/ships/speed.png" height="200" title="Example of a speed vessel">
    <img src="resources/ships/speed_2.png" height="200" title="Example of a speed vessel">
    <img src="resources/ships/speed_3.png" height="200" title="Example of a speed vessel">
</p>

- **Support vessel**

<p align="center"> 
    <img src="resources/ships/support.png" height="200" title="Example of a support vessel">
    <img src="resources/ships/support_2.png" height="200" title="Example of a support vessel">
    <img src="resources/ships/support_3.png" height="200" title="Example of a support vessel">
    <img src="resources/ships/support_4.png" height="200" title="Example of a support vessel">
</p>


