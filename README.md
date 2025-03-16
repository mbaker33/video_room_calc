# video_room_calc 
Video Room Calculator for Cisco video devices by Joe Hughes (beta)
https://collabexperience.com 

### Release Notes:

**v0.1.510**
- Added help button directing users to the new [Video Room Calculator discussion (Webex Space)](https://eurl.io/#4d-kKP6l1) . 
- Optimized for use on Cisco Desk Pro and Board Pro as a web app by adding in timers/delays. 
- Fixed bugs.  

**v0.1.509** 
- Added support for experimental [Workspace Designer](https://www.webex.com/us/en/workspaces/workspace-designer.html) **Custom Rooms** cross-launch.
  - Steps:
    - Requires Cisco network/VPN to reach Workspace Designer internal test site. 
    - Draw your room in the Video Room Calc.
    - Click on the upper right corner cube icon.
    - Internal Workspace Designer opens in a pop-up tab.
  - https://collabexperience.com checks to see if the internal Cisco site is accessible before opening: 
      - If not accessible, ** **Requires a Cisco network connection.** ** label is shown in red. 
      - If not accessible, the cube icon will be grayed out but still enabled.
      - All buttons work regardless of messages since the user could make a VPN connection at any moment without the browser knowing. 
  - Not all devices in the Video Room Calc are supported by the Work Space Designer. 
- Color and Role added to **Details** --> **Items** 
  - Feature mostly applicable to experimental **Custom Rooms** feature. 
  - Color changes the color in the Workspace Designer only and not the Video Room Calc.
  - Role changes the screen role or camera role value on the Workspace Designer.
  - PTZ 4K camera roles include Cross-view, Extended Reach or PresenterTrack. The FOV on the VRC canvas will change based on these roles. 
    - **Caution: **  It is possible to create combinations of **roles** for the display and/or cameras that are not supported by the actual video devices.
- Added Board Pro G2 55 & 70 model Floor Stand models.
- Change display width between 65" to 85" for the Room Kit EQX and Room Kit EQX Floor Stand Model  
    - Please be aware that not all 85" displays will fit in the Room Kit EQX.  75" is a safer size if displays are untested. 
- Removed device type _Room Kit EQ: Quad Cam + PTZ 4K Extended_. The Room Kit EQ: Quad Cam and the PTZ 4K camera can be added separately and work better if used with Workspace Designer. 
- New objects: Laptop, Plant, Wheelchair, accessibility block, accessibility wheelchair 
- Created a [Video Room Calculator discussion (Webex Space)](https://eurl.io/#4d-kKP6l1) 
- In support of the **Custom Rooms**, the Label field with JSON is inserted direct into the Workspace Designer: 
  - Anything not in curly brackets ({}) is ignored.
  - Examples: 
    - For walls, glass walls or boxes: {"color":"#FF0000"}, {"opacity":"0.5"}
    - To flip a PTZ 4K camera: {"scale":[1,-1,1]}
    - To change a person model use {"model":"man-standing-pen"}.  Default person is {"model":"woman-standing"}. 
    - To changed the x, y, z rotation of any object: {"rotation":[0, 3.14, 0]}
      - Rotation is in radians.
      - Overrides the Degree field.
  - Example with JSON in the **Details** --> **Item:** **Label** field: [Video Room Calc Labels with custom JSON](https://collabexperience.com/?x=A1v0.1.510b1000c1000~Video+Room+Calc+Label+JSON+example~B000101AG632a333b623~%7B%22scale%22%3A%5B1%2C-1%2C1%5D%7D~WA125a52c33e864~%7B%22color%22%3A%22red%22%2C+%22opacity%22%3A%220.5%22%7D~WD522a626b70c200e200j200~%7B%22color%22%3A%22blue%22%2C+%22rotation%22%3A%5B0.785%2C0%2C0.785%5D%7D~)
  - **Caution:**  Labels are powerful but can create undesired results.
- Not published to GitHub.
- Fixed some bugs, added some bugs. 

**0.1.508**
- Major improvements to **Details** --> **Settings:** **Background Image** 
- Added informational tabs: **Legend, Templates, Resources** and **Disclaimer**. Coding work done by Mark Baker. 
- Not published on GitHub. 

**v0.1.507**
- If you load a Shareable Link, the Video Room Calculator will automatically convert it to your last unit used, meters or feet.  To turn off go to **Details** --> **Settings:**
- Added support for **Details** --> **Settings:** **Snap to Objects**. 
- Added support for **Details** --> **Settings:** **Snap Center to Increment**.
- Added support for **Details** --> **Settings:** **Background Image**
- Added a Box object. 
- Added a Label field to **Details** --> **Item**
  - Label field will be used for future label feature.
- Narrow width field added to tapered/trapezoid tables.
- Not published on GitHub. 


**v0.1.506**
- Added Table Navigator & Wall Navigator. 
- Added field Item Height to Tables, Walls and Columns.  
- Added tool tips/info bubbles. Hover over underlined text. 
- Fixed a major bug.  On first load, if a Video Room Calculator URL was refreshed 2x without doing any changes, there was a chance objects would delete. 
- Cleaned up some old code, mostly related to SVG which is no longer used in favor of Konva.js & canvas. 

**v0.1.505 (not published)**
- Added new sub-tabs under Details —> Items, Room, Settings
- Added new fields: **Room Height**, **Software Experience** and **Version / Author** on the **Details —> Room** tab.  These fields are informational and don't change the Video Room Calc drawing. 
- Added Door Left, Door Right, Double Door objects. 
- Added Corner Radius / Corner Radius Front Half for Rectangle Tables. 
- Added Position Z (to base of object)
- **Shortcut keys:**
  - ctrl-d / cmd-d = duplicate 
  - ctrl-z / cmd-z = undo
  - ctrl-y / cmd-y = redo 
  - Delete / Backspace = delete items
  - up, down, left, right arrows = moves a _**single**_ item (does not move multiple selected items). 

**v0.1.504**
- Added Walls, Glass Walls, Column rectangle, Standing Person objects. 
- Added Height to each item. Height does not show up on the canvas rendering but is used for reference.  The assumption is that height is the bottom of most items to the ground (e.g. Quad Camera). For Walls, Glass Walls and Columns, it is assumed the item is touching the ground when height is measured.
- Updated the rotator anchor from a rectangle to a circular arrow. 
- Fixed a major bug that could cause items to delete when zoomed in and clicking an update button. Undo button was your friend before this issue was fixed. 

**v0.1.503**
- Added [Cisco Ceiling Microphone Pro](https://www.cisco.com/c/en/us/products/collateral/collaboration-endpoints/collaboration-peripherals/ceiling-microphone-pro-ds.html).
- Updated license from MIT to MIT NON-AI. 
- Added extra links to resources. 

**v0.1.502**
- Full URL query string in address bar now updated dynamically with changes. Copying address bar is similar to clicking on Shareable Link.
- Shareable Link now copies a hyperlink that is name of the room.  If the room does not have a name, then "Video Room Calculator" is used.
- RoomOS QR code now automatically updates with changes. Updates are delayed 2-5 second for performance reasons.  QR code blurs during updates.  The QR code is designed for RoomOS web apps on the Board Pro or Desk Pro. QR Code is also accessible in any browser by adding '&qr' to query string parameter.  
- Improvements to Quick Setup menu to keep confusing things from happening.

**v0.1.501**
- Added template examples. 
- Added QR Code for Shareable Link. Only visible on RoomOS.
- Slightly more complex video devices supported where camera and microphone are not located in x/y center of device. Added Room Kit EQX Floor Stand. 

**v0.1.5**- 
Huge update: 
- Switched from HTML SVG to HTML canvas. Using Konva.js to select and transform images. 
- Drag and drop.
- Multiple Microphones.
- Multiple Cameras.
- Multiple video devices. 
- Multiple Tables. Resizable.
- Chairs. 
- Undo / Redo. Zoom. Pan. Delete. 
- Toggle "guidances" on/off.
- Replaced SVG file download with ability to download a transparent PNG.
- Backwards compatible with v0.1, except for custom cameras.  Shareable Link URLs created in v0.1 with a custom camera or v0.0 redirect to an archive of the previous version. 

**v0.1** 
(circa 10/2023) Updated table / camera FOV based on more accurate data. Picture  SVG based. 

**v0.0** 
(circa 9/2023) First release.  Table / camera FOV and distances only. Picture SVG based. 

### License/Attribution 
- Google Fonts: https://fonts.google.com/ license can be found at https://fonts.google.com/attribution
- Konva.js: MIT license can be found at https://github.com/konvajs/konva/blob/master/LICENSE
- DOMPurify: https://github.com/cure53/DOMPurify license can be found at https://github.com/cure53/DOMPurify/blob/main/LICENSE
- kazuhikoarase QR Code Generator: https://github.com/kazuhikoarase/qrcode-generator 

### Roadmap / ideas
There is no warranty or guarantee the below features will ever be added. 

- Add ability to make FOV, audio and displa shading invisible per a device.
- Outerwalls to snap better. 
- Further shorten URL when an item repeats itself. Decode of this already works, so only the encoding needs to be one. 
- Export configuration to JSON file / Import JSON file. 
- Add label fields that show up on the canvas. 
- Add arrow commands that move more than 1 object. 
- Add other room objects. Add a ceiling layer that can be toggled off/on. Requires additional group/layer. 
- MTR only devices to be labeled or selectable.  
- Remove dependency on Google Icon/Fonts to shorten download time. 
- Remove dependency on DOMPurify and maintain security.
- Ability to change colors for accessibility purposes. 
- Simulated view from camera (simple 2d view of single person zoom and 2 person zoom).
- Add a PoE calculator for the mics, Navigator and PoE cameras. Include different Cisco switches. 
- Add lobes to the digital microphones. 
- Have smaller devices like microphones auto-scale up in size for large rooms. 
- Ability to add custom generic devices.  Speakers, microphones and displays. 

This is a side project. Work is done nights, weekends and holidays.  As of Sept 15, 2024 I'm taking break for a few weeks. 

### Special thanks to those who have tested, gave feedback or were just really patient.
- Tanguay Team - JVV, LT, Clay, Troy, Robbie, Brian, Clarence, Matt, Mike 
- Win.
- Alexis B. 
- Bobby McGonigle. 
- Mark Baker 
- Julie, Anna, Paul & Joshua
- Those who wish to remain anonymous
- The Famous One
- *Thank you to everybody who gave feedback or said thank you.*

_Spelling errors, typos, unused functions, incomplete commenting are all purposly inserted as proof this is not written by AI._ 









