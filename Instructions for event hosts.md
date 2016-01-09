##Instructions for event hosts

###Step 1:
Create a free account on [FreeBoard.io](https://freeboard.io) and create your first board.

###Step 2:
Click add data sources and select Dweet.io from the list

###Step 3:
Enter a unique id for your event.  This must be unique and it will be given out to your competitors.
![](http://i.imgur.com/8KN4xjD.png)

###Step 4:
Add two panes, click the spanner icon, make it 1 column wide and name them 'Left Lane' and 'Right Lane'
![](http://i.imgur.com/iQFKr3N.png)

###Step 5:
Click the plus sign on one of the panes and select 'Indicator Light'
![](http://i.imgur.com/3h8VPRH.png)

###Step 6:
Fill in the desired fields and add a data source.  Data sources and recommended widget types are listed below to help you
![](http://i.imgur.com/UdlBcbI.png)

###Step 7:
Give the site and the unique id from step 3 to your competitors

###The following variables are avalable to be used
####Left Lane
#####Text Widgets
```
datasources["Dweet.io"]["leftUserName"]
datasources["Dweet.io"]["leftLaneDistanceFromRaceReady"] .toFixed(1)
```
#####Indicator Light Widgets
```
datasources["Dweet.io"]["leftLaneOverStaging"]
datasources["Dweet.io"]["leftLaneStaging"]
datasources["Dweet.io"]["leftLanePreStaging"]
```

####Right Lane
```
datasources["Dweet.io"]["rightUserName"]
datasources["Dweet.io"]["rightLaneDistanceFromRaceReady"] .toFixed(1)
```
#####Indicator Light Widgets
```
datasources["Dweet.io"]["rightLaneOverStaging"]
datasources["Dweet.io"]["rightLaneStaging"]
datasources["Dweet.io"]["rightLanePreStaging"]
```
