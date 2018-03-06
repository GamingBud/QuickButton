# QuickButton
---
With QuickButton, you can simply send a single line message to have a button created. It includes press_detection and mouse-over highlighting. A message will be sent back to your script when the button is pressed. This allows you to complete necessary actions fluidly.

Current functions as of 0.2:  
* Create_Button  
* Delete_Button  

Use:  
* Create_Button: msg.post("Quick_Button.gui", "Quick_Button", {order = order, pos = pos, font = font, text = text})
* Delete_Button: msg.post("Quick_Button.gui", "Delete_QB", {Button num})  

Upon click, Quick_Button.gui will send a message back to the owner of the button in question, which will be sent as:
* message_id = order attached to button on creation, message = Button number, which is iterated in chronological order. 1 is the first button created, 2 is the next, etc.

---
# Version 0.2

Added: Delete_Button, now allowing a single message to be sent to delete all code related to the button in question. Thanks to britzl for bringing to attention that I overlooked the fact that GUI cannot be deleted from another GUI script. 

Various simplifications and modifications.  

Fixed: game.input_binding being overlooked in the example file transfer.
