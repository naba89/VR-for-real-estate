#Virtual Reality Land Viewing
1. Problem Statement chosen:
  - Make property walkthroughs more interesting
2. Solution:
  - One app on Pk’s phone that allows him to see the land in a 3D perspecyive through his google cardboard
  - Another app on his co pilot’s tab which shows the land in as  2D image, and zooms in only into the part that PK is viewing
3.	Technology Stack Used:
  - Unity for 3D viewing of land on PK’s phone
  - Alljoyn for communication between the devices
  - Android java for the rest
4.	Solution design:
  - A Unity App takes care of producing a 3D view using a picture got from the database.
  - At the same time it acts a server which sends the x,y coordinates of view point to the client (tablet)
  - The x,y cordinates are sent everytime the 3D view is updated
  - The x,y coordinates are sent via Alljoyn Framework hence facilitating data transfer between heterogenous Operating Systems
  - One the x,y coordinates are received on the client end, a scroll is performed on the image on the tablet app, hence highlightening on the area that is being veiwed in the 3D app.
5. Future enhancement:
  - When the tablet wants to communicate with the unity app, a touch needs to be made on the tablet app, the coordinates of touch are communiated to the 3D app, and a arrow is drawn on the 3D view indicating the user to turn in the specified direction
								
