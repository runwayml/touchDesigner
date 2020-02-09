# Enhance Textures

Generation of realistic textures using **ESRGAN** models for image
super-resolution. This example reads low resolution textures, enhances
them, and sends its output to TouchDesigner.

# Requirements:
Requires Touchdesigner build 2019.30790 or newer (SocketIO DAT added)

### Running the Example

* Download the project folder.
* Open Runway and create a workspace with the ESRGAN model. Check the [docs](https://docs.runwayapp.ai/#/) for tutorials and additional information.
* Select **Network** and **Socket.io** to review the Socket.IO Server details.
* Run the model.
* Open the **EnhanceTextures.toe** file and press 'F1' to enter performance mode.
* Click on the `Port` field and input the port from Runway's Socket.IO Server address (default is `3000`).
* Click on the document icon 📄 next to the `File` field and select any texture from the `/images` subfolder.
* Wait until the upscaled image is rendered.
* Press 'Esc' to leave performance mode.

![EnhanceTextures Preview](preview.png)

**Notes:** 
* If the example does not display the upscaled texture, in Touchdesigner, navigate to `Runway_ESRGAN` > `texture_viewer`, and find the `socketio` DAT. Click on `Reset`.
* The textures in the `/images` subfolder are part of the [mini8x texture pack](https://forum.minetest.net/viewtopic.php?f=4&t=14633) by [D00Med](https://github.com/D00Med) (Licensed under CC-BY-SA 3.0).

### Add Your Own Images

* Try adding your own files to the `/images` subfolder, or use the file browser to find them.
