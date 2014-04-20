Using G8 in Your Host
=====================

Ableton Live
------------

.. image:: /images/abletonRouting.png

**MIDI In to G8**:

- Add an instance of G8 to an audio track that you want to apply gating to. 
- Create a MIDI track. Optionally, create a clip with the pattern that you want to use for gating. 
- Click the “IO” symbol on the right side of the Ableton window to show the input/output section for each track.
- Go to the created MIDI track, and select the “MIDI To” dropdown, selecting your audio track that G8 is using. 
- The subcategory dropdown menu right below this should now activate allowing you to select “1 G8 Gate.” Selecting G8 will route the MIDI track into G8 so that you can use it to control the gate’s envelope. Make sure to set G8’s MIDI input note is set to whatever note is being used in your pattern.

**MIDI Out from G8**:

- Add an instance of G8 to an audio track. 
- Create a MIDI track.
- Click the “IO” symbol on the right side of the Ableton window to show the input/output section for each track.
- Go to the created MIDI track, and click the first “MIDI From” dropdown, selecting your audio track that G8 is using. 
- The subcategory dropdown menu right below this should now activate allowing you to select “1 G8 Gate.” Selecting G8 will route the MIDI from G8 into this track.
- Set "Monitor" to "In". This will enable MIDI to reach this track, even when it's not set to record.

**Sidechain Ins**:

- Add an instance of G8 to an audio track that you want to apply gating to. 
- Create a second audio track with the clip you want to use as a sidechain. 
- Click the “IO” symbol on the right side of the window to show the input/output section. 
- Go to the sidechain track, and select the “Audio To” dropdown, changing “Master” to your main audio track. 
- The subcategory dropdown menu right below this should now activate allowing you to select “3/4 G8 Gate.” Activating this setting will route the sidechain track into the third and fourth inputs on G8 so that you can use it to control the gate’s envelope.

**Reject Outs**:

- Add an instance of G8 to an audio track that you want to apply gating to.
- Create a second audio track for receiving audio from G8's Reject Outs.
- Click the "IO" symbol on the right side of the window to show the input/output section.
- Go to the track that is receiving audio from the Reject Outs, and click the first dropdown box under "Audio From". From here, select the track that G8 is on.
- The second dropdown box will now allow you to select "G8 Gate 3/4".
- Set "Monitor" to "In". This will allow you to always hear the audio coming from G8's Reject Outs.


Bitwig Studio
-------------

**Sidechain Ins and Reject Outs**:

Unfortunately, Bitwig does not support routing to or from multi-channel plug-ins at this time. When Bitwig is updated, we will update this manual to provide instructions on how to use it.

Cubase
------

Digital Performer
-----------------

FL Studio
---------

Logic Pro X
-----------

Max/MSP
-------

.. image:: /images/maxMSPRouting.png

**Sidechain Ins and Reject Outs**:

Due to the modular, visual nature of Max/MSP, it is extremely easy getting setup with G8's routing.

- Create a "vst~ 4 4" object. The "4 4" argument means that the plug-in will have four inputs and four outputs.
- Create a message object (hit 'm' to create one quickly). Write "plug" (no quotes) in this message box. Connect it to the first input of the vst~ object.
- Click the "plug" message. It will bring up a window to load a plug-in on your hard drive. On OS X, this will be under /Library/Audio/Plug-ins/VST/Unfiltered Audio/. We recommend using the VST version in Max/MSP.
- Create a message object, this time called "open". This message object will allow you to see your interface.
- The first two inputs of the vst~ object are the main ins, while the second two are the sidechain ins.
- The first two outputs of the vst~ object are the main outs, while the second two are the reject outputs.

**MIDI**

Using MIDI in Max/MSP is outside the scope of this manual. The above instructions will help you to get G8 loaded and running. For an interactive guide to using automation with the vst~ object, hold "alt" and click the vst~ object while the Max patching window is unlocked.


Numerology
----------

REAPER
------

Renoise
-------

Studio One
----------

**Sidechain Ins and Reject Outs**:

Unfortunately, Studio One does not support audio routing to or from multi-channel VST2 plug-ins. We plan on releasing a VST3 version of G8 in the future. This will be a free update to all users.

.. image:: /images/studioOneMidi.png

**MIDI**:

Routing MIDI to and from G8 is extremely easy in Studio One.

- Add G8 Gate to an audio track.
- Create an instrument track.
- For receiving MIDI from G8, click the MIDI input selector (the top one) and select G8 Gate channel 1.
- For sending MIDI to G8, click the MIDI output selector (the bottom one) and select G8 Gate channel 1.
