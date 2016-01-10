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

###[Here is how I setup my staging site](https://freeboard.io/board/2KJsA8)

###Step 7:
Give the site URL and the unique id from step 3 to your competitors

###The following variables are avalable to be used
####Left Lane
#####Text Widgets
This is the competitors name in the left lane
`datasources["Dweet.io"]["leftUserName"]`

This is how far in metres the are from being race ready
`datasources["Dweet.io"]["leftLaneDistanceFromRaceReady"] .toFixed(1)`

#####Indicator Light Widgets
Over staging - ie Too far foward
`datasources["Dweet.io"]["leftLaneOverStaging"]`

Ready to race - ie Car is staged
`datasources["Dweet.io"]["leftLaneStaging"]`

Pre-staged - ie on the strip and F11 or F12 has been pressed to indicate their lane
`datasources["Dweet.io"]["leftLanePreStaging"]`


####Right Lane
#####Text Widgets
This is the competitors name in the left lane
`datasources["Dweet.io"]["rightUserName"]`

This is how far in metres the are from being race ready
`datasources["Dweet.io"]["rightLaneDistanceFromRaceReady"] .toFixed(1)`

#####Indicator Light Widgets
Over staging - ie Too far foward
`datasources["Dweet.io"]["rightLaneOverStaging"]`

Ready to race - ie Car is staged
`datasources["Dweet.io"]["rightLaneStaging"]`

Pre-staged - ie on the strip and F11 or F12 has been pressed to indicate their lane
`datasources["Dweet.io"]["rightLanePreStaging"]`
