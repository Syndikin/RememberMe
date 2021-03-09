# RememberMe

## Description
This is an application that is designed to make every day task easier for the person on the go. It is designed with a simple user interface and easy to use features. The goal is less is more. This application is a reminder app that features location based reminders based on proximity. The application will take user inputs into a to-do list type interface. The user will input a reminder i.e pick up oranges then will input under location the store that they wish to go i.e Walmart. The application will then pull search results from google maps of the nearest Walmarts and pormpt the user to pick the desired one. After the location of the to-do list item is selected, the user will be prompted to choose the proximity of which they wish to be alerted. The application will request access to user gps and track location til the to-do list item has expired or has been completed by user.

## Conceptual Design (DRAFT)
![Alt Text](https://github.com/Syndikin/RememberMe/blob/main/WireFrame1.JPG)
![Alt Text](https://github.com/Syndikin/RememberMe/blob/main/WireFrame2.JPG)
![Alt Text](https://github.com/Syndikin/RememberMe/blob/main/WireFrame3.JPG)
![Alt Text](https://github.com/Syndikin/RememberMe/blob/main/WireFrame4.JPG)
![Alt Text](https://github.com/Syndikin/RememberMe/blob/main/WireFrame5.JPG)

## Requirements & Use Case

## User Story:
As a person who is always on the go and with an endless amount of errands to run. 
I need an application that will help me complete these items.  I would like to be alerted within a proximity of my desire and I would like alerts to be sent to my phones homescreen. I also would like to choose the location of  where I would like to complete my item and the choice to put an expiration date on the item.
I am also not tech savvy and need a simple interface I can navigate.

## Use-Cases:
The user will be able to create new To-do list are desired. The user will be able to link each item to a location. 
The user will have the flexibility to set radius of alerts and an expiration date on items in their to do list. 
The user will also be able to view current active To-do list and edit To-do list as desired.

## UML Sample: 
![Alt Text](https://github.com/Syndikin/RememberMe/blob/main/UMLSample.jpg)

## Requirements:
|ReqId| Requirement Details| Test Method| testID|
|---|---|---|---|
|1| The system shall allow user to create new to-do list.|test| 100|
|1.1| The system shall allow user to review active to-do list.|test|101|
|1.2| The system shall allow user to input and delete new items on to the to-do list.|test|102|
|1.3| They system shall accept desired location of to-do list item.| analysis| N/A|
|1.3.1| The system shall be able to correctly identify locations inputed by user.| test |103|
|1.3.2| The system shall request a desired alert radius based on current location.| inspection| |
|2| The system shall properly retrieve user's location within 0.1 miles.| inspection|test |200|
|2.1| The system shall have capability to use the user's location provided by the user's browser.|test|200|
|2.1.1| The system shall request permission to use the user's location if not already given.|inspection|N\A|
|2.1.2| The system shall be able to use GPS coordinates as an alternate method of location tracking.|test |201 | 
|3| The system shall be able to calculate the approximate distance between the user's current location and the location of the to-do list item.|analysis | |
|3.1| The system shall provide appropiate alert to user's homescreen when in proximity of item.| inspection| |
|3.1.1| The system shall allow user to check off to-do list item and deactive it.|inspection| |
|4| The system shall allow user to input an expiration date on to-do list item.|inspection| |
|4.1| The system shall deactive to-do list item upon expiration date.|test| |
|4.1.1| The system shall provide an alert of deactived to-do list item.|test| |
 
## Testing

|testID|ReqID|Test requirement|status|Date completion|
|---|---|---|---|---|
|100|1|To-do list created accurately according to template|not tested|TBD|
|101|1.1|To-do list are recorded and saved properly for user reference|not tested|TBD |
|102|1.2|All editing functions on To-do list interface are active and working properly|not tested|TBD|
|103|1.3|Nearby item locations properly generated using google maps|not tested|TBD|  
|200|2| user location accurate and within a 0.1 mile radius|not tested| TBD|
|201| 2.1.2| System can use GPS location as alternate location tracking method| not tested| TBD|
|300| | | | |
|400| |To-do list deactives properly upon user completion| not tested| TBD|
|401|4.1|To-do list deactives upon expiration date| not tested| TBD|
|402| 4.1.1|To-do list alerts user of deactivation| not tested| TBD|


