Ahmedabad_CityMatrix

Step_01

Prior to running the R06 files please download Rhino 06
Licensed evaluation version is available at the link below, 

https://www.rhino3d.com/download/rhino-for-windows/6/evaluation

Once you have downloaded rhino 06 you will find the command line above 
enter in "grashopper" 

If all runs smoothly then procede to step 02

Step_02

Download the gHowl and Firefly files, run firefly intial. 
The gHowl is a component to be added to grasshopper 

Open grasshopper, go to files 
   -special folders 
   -components folder 
   -place the component and the .dll file and unblock them from        properties 

Step_03 

Run the Rhino file and run the gh script. 
OSC reader will not function initially until setup. 

Step_04 

Create OSC app or download one from an online webstore. 
We are currently using TouchOSC available on both iOS and Android 

Step_05 

Set up the listening ports and the IP address to natively listen to then script should the activate all components from red to green. 

I have attached a processing script for OSC listener. Though I suppose you will need to find a work around incase the app is not possible. 

Step_06

Run basic_pd in pd extended and adjust udp values accordingly and local IP address for outgoing and incoming messages to listen for in grasshopper using either firefly firmata or ghowl. 

This project has taken inspiration and understanding from MIT Media Lab projects at Senseable CityLab. 

Check out Media Lab GITHub by Ryan, Link attached below, 

