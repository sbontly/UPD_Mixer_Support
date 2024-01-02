# UPD_Mixer_Support

 Supporting Files for the UP Deko Mixer

 -------------------------------------------------------------------------
 Audio.tox:

 WARNING: not the prettiest or most optimized application, but it works

 - This file externalizes the audio analysis from the mixer, allowing for the computation to be done on another CPU core.

 1) click "Open Pars" to setup configuration:
    - Active: this enables the output of the data being set to the mixer
    - Open Audio Out Parameters: This will allow you to hear the music being analyzed through an output device, only necessary if using a local track
    - Hz: How frequent the data is analyzed. Be careful how much resolution is used as it is resource intensive
    - Open Audio In Parameters: This will allow you to select the unput source for the audio
    - Open Preset Manager: ADVANCED, only for use with TouchOSC, but not really needed to mess with as it is setup for making presets
    - TouchOSC IP: This is the IP of the device running the TouchOSC interface that works with the mixer
    - TouchOSC In Port: This is the port that the TouchOSC app will listen to show the current values of your configuration
    - TouchOSC Out Port: This is the port the The TouchOSC app will send the data to manipulate the audio analysis
    - Receiver IP: This the IP of the Machine the Mixer is running on
    - Receiver Port: This is the port that the mixer is listening to
    - Send touchOut Audio: This enables a touchOut CHOP to send to another TouchDesigner Application not related to the mixer
    - Use Track: Switches the audio analysis to a track located on you local harddrive
    - Track: The path to the local track
    - Reset: Resets the track being played
    - Play: Starts the local track


 ------------------------------------------------------------------------

TouchOSC:

- Custom UI to work directly with Audio.tox
- This communicates across a network via OSC
- IN DEVELOPMENT: Page 2 provides a remote connection for overall use away from the machine running the mixer
-------------------------------------------------------------------------

MIDI:

- Native Instruments Tractor Kontrol F1 controller mapping configuration
- This connect directly into the UP Deko Mixer, enabling fast GUI navigation and the custom MIDI mapping experience

---------------------------------------------------------------------------

Point Clouds:

- pointCloudBuilder - a simple builder file for custom point clouds
   - Directory: File path where you want to save the files
   - Index: Keeping an index to order the files for use in the mixer, directly relates to chosen point cloud file
   - File Name: The name of the point cloud
   - Extension: File type, it is preffered to use .exr until a better understanding of optimization is known
   - Save: Once all the parameters are set above, and the 3D model has been setup inside the network, press this button to create a folder in directory with all needed assets



