# video_room_calc
**Video Room Calculator for Cisco video devices by Joe Hughes** (beta)
https://collabexperience.com

Please see the [FAQ](https://github.com/vtjoeh/video_room_calc/blob/main/FAQ.md).

### Release Notes:

**v0.1.611** 🥳
- **Workspace Designer Customs Rooms** integration is now publicly available. 🎉🎉🎉🎉
- Labels now show on room canvas by using the Labels toggle button. 🏷️
- Camera coverage has been updated to more closely reflect the Workspace Designer and/or incorporate the Virtual Lens settings. 📸
- Virtual Lens is shown on the Room Bar Pro & Board Pros. Lens 1 coverage shows the wide lens, Lens 2 coverage shows the tele-lens, and Lens 3 shows the virtual lens.
- `PTZ 4K camera` object has been updated to `PTZ 4K Camera + Mount` to better match the Workspace Designer object. The older PTZ 4K camera (non-mount) can be found under Workspace Designer's partially/non-supported items. Previous designs won't be affected.
- Door renderings in the Workspace Designer are now double thickness by default to show on both sides of a wall. Previous designs won't be affected. 🚪🚪
- Added ability to swap out similar type objects and maintain attributes like X, Y, Z from the individual items page.  For example, swap a Room Bar for a Room Bar Pro to see the coverage differences.   📸 🔄 📷
- Quick Setup automatically adds chairs around the table. 🪑+🪑+🪑+🪑
- Bug fixes, template updates and other minor changes.

**v0.1.610**
- Fixed Edge browser added an image search button to certain images.
- Added Room Name to quick setup.
- Added extra delay to tooltips.

**v0.1.609**
- Title removed from room canvas to make more space for the actual room.

**v0.1.608**
- Minor bug fixes including update of Ceiling Mic Pro ceiling mount.
- updated templates.

**v0.1.607**

* **Default Wall:** A default wall is now shown on the main room canvas. This can be removed with the **Remove Default Walls** toggle and is reflected in the Workspace Designer.
* **PTZ mount options:** Added mount options for PTZ cameras: Standard, Flipped, and Flipped & Ceiling Pole, which are rendered in Workspace Designer. 📸💈
* **Ceiling Mic Pro Ceiling mount options:** Show the ceiling wire mount.
* **Tilt & Slant:** Introduced Tilt and Slant options for Workspace Designer (public integration release in June). These features are disabled by default; enable them under Details → Settings. If a Shareable Link has Tilt or Slant configured on an item, the fields will be applied regardless of the **Workspace Designer Tilt and Slant** settings. Since the Video Room Calc does not reflect the changes made by Tilt or Slant, these settings remain disabled by default. 🙂🙃
* **New Devices:**
  * **Row of Chairs:** Added a resizable Row of Chairs shape for quickly creating multiple chairs. 🪑🪑🪑
  * **Couch:** Resizable couch. 🛋️
  * **Curved Table:** New Curved Table designed for use with Campfire setups. Enable this under Details → Settings: **Workspace Designer non-supported items**. ⛺️🔥
* Minor bug fixes: Improved multi-select functionality with shortcut keys. 🔧

**v0.1.606**
- 	**🟨Highlight Small Devices🟨** You can now highlight and move any device smaller than 0.5m/1.6ft! Resizable objects like walls remain unaffected. Please note that the highlight small device setting is not saved in the shareable link.
- **Ellipsis Menu Added to Toolbar:** A new three-dot (…) ellipsis menu has been added to the toolbar. The drawing features Snap to Objects and Snap Center to Increment have been moved to this menu. Highlight Small Devices can now be found there. 🔵🔵🔵
-	**🔽Minimize Menu🔼** You now have the ability to open and close the menu, which helps optimize screen real estate on both desktop and mobile. 📱💻
- **Draggable Coverage Menu:** Mic, Display, and Camera coverage menus (activated by holding down the perspective button) can be dragged if needed to temporarily see more of the room canvas. 🖼️ 🎥🎤
- Small bug fixes. 🐞
- For an overview of features, see the Vidcast [Video Room Calc v0.1.606 feature overview](https://app.vidcast.io/share/619c0bd1-7b9e-487c-be5a-afd7c3454ad3)

**v0.1.605**
- Quick Fix: Google search occasionally displayed a legacy URL query string format that, when clicked, resulted in a redirect to version v0.0 of the Video Room Calculator. This issue occurred because, when the Video Room Calculator site is unable to parse a legacy version, it redirects users to a backup site to ensure that your data is not lost.

**v0.1.604**
- shift+ctrl+z/shift+cmd-z now works as an Undo shortcut. The previous shortcut of ctrl-y/cmd-y still works. ↪️
- A blank default room size will no longer appear as a URL queryString parameter, as it is unnecessary.
- Maximum width for control button group above the room canvas has been set to 850px for better support with wide displays.
- A bug has been resolved where the undo function did not update the Shareable Link URL until another action was performed.
- Additional minor changes have been implemented. 😊✨

**v0.1.601, v0.1.602, v0.1.603**
- Duplicating chairs [ctrl-d] spaces them evenly for quicker chair setup 🪑✨
- Fixed tooltip overlaps & other minor issues 🔧

**v0.1.600**
New Features:
- Major UI/reskin changes 🌟🌟🌟
- Moved templates and Quick Setup menu to New dialog window 🆕
- Visiting https://collabexperience.com/ (no shareable link querystring parameters) automatically opens the New dialog window.
- Added right-click menu for copy, paste, delete, etc. 📋✂️🗑️
- Ctrl-R/Cmd-R to rotate 🔄.
- Update/Down/Left/Right arrows now move multiple items ⬆️⬇️⬅️➡️.
- Ability to see individually selected and unselected items highlighted in blue when using shift+clicking on items 🔵.
- `Esc` key to unselect all items ❌.
- To get details on an object, now use single click and instead of double click. 🎯
- Cam, mic, and display reach buttons now discreetly toggle their perspective settings to keep the canvas cleaner (Power user's - click and hold for 1 sec on the cam, mic, or display buttons to turn the shading on/off for individual devices) 🎥🎤🖥️.
- Removed items from the default Equipment list that are not supported in the Workspace Designer 🧊. They can be added back in by the power user Details —> Settings —> Workspace ⚙️.  Workspace Designer integration still requires a Cisco VPN

**v0.1.515, v0.1.516**
- Items off stage no longer show up in the URL, Shareable Link or Workspace Designer Custom Room. Items off stage are still there during multi-item drag & drop or room resizes.
- Code optimization.

**v0.1.514**
- Added warning when a 2nd video device (not camera) is added to the room canvas.  The **PTZ 4K** camera on the below picture is actually a **Room Kit EQ: PTZ 4K Camera**
- Reduced Quick Setup items in the video devices menu.
- Bug fixes.
<img width="275" alt="image" src="https://github.com/user-attachments/assets/def64fdf-e553-482f-92b9-5452e5444cbc" />

**v0.1.513**
- It is now possible to disable the camera FOV, audio reach, or display reach for a single object. Simply double-click on the object on the Video Room Calc canvas and three new buttons will appear next to the Update Item button.
<img width="312" alt="image" src="https://github.com/user-attachments/assets/4ddda88d-891b-4873-bb88-0fbc38581ae1" />

- **Stage Floor:** A new object called Stage Floor has been added. It can be found under **Equipment** -> **Furniture** -> **Stage Floor.** The Stage Floor is similar to the Box object, but stage floor always remains at the lowest level on the room canvas. This is useful when creating a custom room with a stage, as Box objects are typically on the same level as Tables and Walls.
- The **Software Experience: MTR or Webex** is now supported for Workspace Designer Custom Rooms. Under **Details** -> **Room** -> **Software Experience:** **MTR** or **Webex**.
- Orphaned objects that are not on the VRC canvas will not be visible in the Workspace Designer export. They will be marked as {"hidden": true} in the JSON.
- The Displays and Cameras now have a read-only **Top Elevation field** making it easier to determine what the base elevation of a camera sitting on top of display should be when working with the Workspace Designer Custom Rooms. Double-click on the object to see this information in the **Details** -> **Item** menu.
- An issue has been fixed where the displays base elevation on export to the Workspace Designer Custom Rooms were too high.  Displays will now be accurately placed. Existing Video Room Calculator designs will need displays's base elevation updated to work properly with the Workspace Designer.
- Bug fixes.

**v0.1.512 (not published)**
- Bug fixes.

**v0.1.511**
- Provide user warning if the URL file size exceeds 8190 characters, which is about 500 objects on the canvas.
- Fixed some bugs related to local storage.

**v0.1.510**
- Added help button directing users to the new [Video Room Calculator discussion (Webex Space)](https://eurl.io/#4d-kKP6l1) .
- Optimized for use on Cisco Desk Pro and Board Pro as a web app by adding in timers/delays.
- Fixed bugs.
- Increased URL size from 4094 characters to 8190.  To date only one person has reported hitting the limit of 4094 characters.

**v0.1.509**
- **Experimental Feature: Custom Rooms** Added support for experimental [Workspace Designer](https://www.webex.com/us/en/workspaces/workspace-designer.html) **Custom Rooms** cross-launch.
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
- In support of the **Custom Rooms**, the Label field with JSON is inserted direct into the Workspace Designer.  See the FAQ for more info.
- Not published to GitHub.
- Fixed some bugs, added some bugs.

**0.1.508**
- Major improvements to **Details** --> **Settings:** **Background Image**
- Added informational tabs: **Legend, Templates, Resources** and **Disclaimer**. Coding work done by Mark Baker.
- Not published on GitHub.

**v0.1.507**
- **Maintain unit feet/meters** If you load a Shareable Link, the Video Room Calculator will automatically convert it to your last unit used, meters or feet.  To turn off go to **Details** --> **Settings:**
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

This is a side project. Work is done mostly nights, weekends and holidays.

### Special thanks to those who have tested, gave feedback or were just really patient.
<sub>* Tanguay Team - JVV, LT, Clay, Troy, Robbie, Brian, Clarence, Matt, Mike </sub> \
<sub>* Win.</sub> \
<sub>* Alexis B. </sub> \
<sub>*  Bobby McGonigle. </sub> \
<sub>*  **Mark Baker** </sub> \
<sub>* Julie, Anna, Paul & Joshua</sub> \
<sub>*  Those who wish to be uncredited</sub> \
<sub>* The Famous One</sub>

_Spelling errors, typos, unused functions, incomplete commenting are all purposly inserted as proof this is not written by AI._









