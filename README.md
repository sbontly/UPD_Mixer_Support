# UPD_Mixer_Support
 Supporting Tox Files for the UP Deko Mixer

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

 F1MidiEmulator.tox: (STILL TO BE UPLOADED)

 - This file acts as a virtual midi controller that mimics the Native Instruments Tractor Kontrol F1

 - It will allow the user to extend the capabiliteis of the mixer to its true potential

 - In the future this asset will become obsolete, since the idea is to prepare the mixer to recieve any MIDI device to control the main features

