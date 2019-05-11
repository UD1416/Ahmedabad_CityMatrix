Ahmedabad_CityMatrix

Version 1.02.01 is out with runtime bug fixes

Step_01

Prior to running the R06 files please download Rhino 06
Licensed evaluation version is available at the link below, 

https://www.rhino3d.com/download/rhino-for-windows/6/evaluation

Once you have downloaded rhino 06 you will find the command line above 
enter in "grashopper" 

If all runs smoothly then proceed to step 02/ if not check Rhino troubleshooter 

Step_02

Download the gHowl and Firefly files, run firefly intial. 
The gHowl is a component to be added to grasshopper 

Open grasshopper, go to files 
   -special folders 
   -components folder 
   -place the component and the .dll file and unblock them from properties 

Step_03 

Run the Rhino file and run the gh script. 
OSC reader will not function initially until setup. 

Step_04 

Create OSC app or download one from an online webstore. 
We are currently using TouchOSC available on both iOS and Android 

Step_05 

Set up the listening ports and the IP address to natively listen to the script, it should then activate all components from red to green. 

I have attached a processing script for OSC listener. Though I suppose you will need to find a work around incase the app is not possible. 

Step_06

Run basic_pd in pd extended and adjust udp values accordingly and local IP address for outgoing and incoming messages to listen for in grasshopper using either firefly firmata or ghowl. 

For Grasshopper and what ever app you may be running as for communication they are required to be on the same network and have their ip addresses configured correctly so that one is a reciever and other sender. 

If the script runs slow cross check poll time for each component, or check network stability. 

This project has taken inspiration and understanding from MIT Media Lab projects at Senseable CityLab. 

Check out Media Lab GITHub by Ryan, Link attached below, 
https://github.com/popabczhang/CityMatrixGH

