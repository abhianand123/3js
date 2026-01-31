==============================================================================
             3D HAND TRACKING PARTICLE ENGINE - SETUP GUIDE
==============================================================================

Hey,

Here is the source code for the gesture-controlled particle system I built. 
It uses Three.js for the 3D rendering and MediaPipe for the hand tracking AI.

Because this project needs to access your webcam and load external libraries, 
you can't just double-click the HTML file to open it (security browsers block 
the camera on file:// paths). You need to run a quick local server.

Here is the easiest way to get it running on your machine:

------------------------------------------------------------------------------
STEP 1: FOLDER SETUP
------------------------------------------------------------------------------
1. Create a new folder on your desktop (call it "particle-engine" or whatever).
2. Inside that folder, create a file named "index.html".
3. Paste the code I sent you into that file and save it.

------------------------------------------------------------------------------
STEP 2: OPEN IN VS CODE
------------------------------------------------------------------------------
1. Open Visual Studio Code.
2. Go to File > Open Folder and select the folder you just made.
   (Make sure you open the whole folder, not just the file!)

------------------------------------------------------------------------------
STEP 3: START THE LOCAL SERVER
------------------------------------------------------------------------------
We need a tiny Python server to fool the browser into thinking this is a live website.

1. In VS Code, go to the top menu: Terminal > New Terminal.
2. In the terminal window at the bottom, type this command and hit Enter:

   python -m http.server

   (If that doesn't work, try: python3 -m http.server)

3. You should see a message saying "Serving HTTP on :: port 8000".

------------------------------------------------------------------------------
STEP 4: RUN IT
------------------------------------------------------------------------------
1. Open Chrome (it works best on Chrome).
2. In the URL bar, type: http://localhost:8000
3. When it asks for Camera Permissions, click ALLOW. 
   (The screen might stay black if you block the camera).

------------------------------------------------------------------------------
TROUBLESHOOTING
------------------------------------------------------------------------------
- If the screen is black: Check the VS Code terminal to make sure the server 
  is actually running.
- If the camera won't start: Check the lock icon 🔒 next to the URL bar and 
  make sure permissions are allowed.
- To stop: Just click inside the VS Code terminal and hit Ctrl+C.

Enjoy!