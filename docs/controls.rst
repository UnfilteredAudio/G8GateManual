Controls
========

Primary Controls
----------------

**Analysis Gain**:
Controls the amount of gain applied to the analyzed audio signal. The analyzed signal is considered separately from the outgoing signal in G8. Because of this, this control does not affect the amplitude of the signal that you can hear.

This applies gain adjustment to the signal being used for analysis but does not have any effect on the level of the output signal being heard. For instance, if the analysis signal is the normal stereo input, applying a large amount of analysis gain will not cause resulting signal to sound louder after passing through. 

**Threshold**:
Controls the level of the gate’s threshold. When this threshold is exceeded by the amplitude of the incoming audio, the gate will open and allow the audio to pass through.

**Gate Meter**:
A non-interactive component that displays the current value of the gate envelope. If you would like to see a more detailed history of the envelope’s value, you can click the “Display Options” button and enable the “Show Gate” parameter, which will then add the envelope to the waveform display.

**Output Gain**:
Controls the amount of gain applied to the outgoing signal from G8. This gain does not affect the analysis levels of the incoming audio.

**Attack**:
Controls the amount of time it takes for the gate to open to maximum amplitude after the incoming audio goes above the threshold. Extremely short values (< ~10 ms) can result in clicks, due to the rapid change in amplitude.

**Hold**:
Controls the amount of time that the gate is required to stay at maximum amplitude for. If the incoming audio drops below the hysteresis point before the hold stage is finished, the hold stage will complete before the release stage begins.

**Release**:
Controls the amount of time that it takes for the gate to go from maximum amplitude to minimum amplitude. This stage occurs after the incoming audio drops below hysteresis, and after the hold stage is completed.

**Reduction**:
Controls the amount of gain removed from the audio signal when the gate is closed. This effectively sets a minimum amplitude for the gate envelope.

**Hysteresis**:
Controls the hysteresis point, often referred to as the “bottom threshold”. The audio signal must drop below this bottom threshold before the gate can close.

**Dry/Wet**:
Controls the balance between the “dry” (unaffected) incoming signal, and the “wet” (affected) outgoing signal. Please keep in mind that the “dry” signal is delayed by the Lookahead value, meaning that it is not a truly bypassed signal. This was done so that the wet and dry signals maintain the same phase.

**Lookahead**:
Delays the signal by a chosen amount to allow the gate’s analysis stage to better predict incoming transients.

**Delay**:
This control is only active when “Cycle” mode is selected (Please see the section on “Alternate Gate Behaviors”). Controls the length of silence inserted between envelope cycles.

**RMS/Peak**:
Selects the analysis type. Use “Peak” for more rapid analysis of signals with many transients (i.e. percussive signals).

**Behavior Mode**:
Selects the behavior of the gate envelope. Choose between “Regular Gating”, “One Shot”, and “Cycle”. Please see the section on “Alternate Gate Behaviors” for more info. 

**Display Options**:
Provides a menu to enable or disable the entire waveform display, or individual components of the waveform display.

Bottom Left Controls
--------------------
**Channels Display**:
Displays how many channels your host currently supports. This number is equal to the number of input channels. You can use this for troubleshooting your setup.

**Expert Mode**:
Toggles whether or not Expert Mode is active. For more information, please see the section on “Expert Mode”.

**Flip Mode**:
Toggles whether the primary outputs and reject outputs are swapped. For more information and techniques, check out “Reject Outputs” and “Flip Mode”.

Bottom Right Controls
---------------------

**MIDI**:
Toggles whether G8’s MIDI inputs and outputs are active. For more information, please see the section on “MIDI”.

**Reject Outputs**:
One of G8’s most innovative features is it’s ability to create “Reject Outputs” when used in four-channel mode. The Reject Outputs are a set of auxiliary outputs that output the sound that is currently being blocked by the gate. If this is hard to conceptualize, mixing together the gated signal and the Reject Outputs will give you back your original signal.

This opens up all sorts of creative mixing possibilities using a technique that we call “amplitude splitting”. This allows you to create non-linear (amplitude dependent) effect chains using any other plug-in you wish.
For a simple example, you could create an amplitude dependent auto-panner. Simply mix the main outs down to one channel, and the Reject Outputs down to another. If you are creating a four-channel mix, this is an easy and flexible surround auto-panner!

For more information on how to connect the Reject Outputs in your DAW, please refer to the section “Using G8’s Sidechain Inputs and Reject Outputs”. If your host doesn’t support G8’s four-channel layout, then please refer to the next section on using the “Flip Mode”.

**Flip Mode**:
When “Flip Mode” is active, the main outputs and the Reject Outputs are swapped. This is useful for a number of reasons. First, if your host does not support G8’s four-channel mode, then this will still give you access to G8’s Reject Outputs. Second, this mode is visible to automation! This allows you to increase the complexity of your Reject Output effect chains by switching between the two modes. Third, it allows you to simply use the Reject Outputs if you have no use for the main outputs.

Why would you want access to only the Reject Outputs? Well, one of our favorite uses of the Flip Mode is to use G8 as a bizarre compressor! To achieve this, activate Flip Mode, and then change the amount of reduction that G8 is using. There are many other wild effects waiting to be discovered in this mode, especially in combination with G8’s alternate behaviors.

**Expert Mode**:
Expert Mode is an optional mode that provides more in-depth control for advanced analysis situations. In this mode, you have access to the gain of each individual channel, along with the ability to filter the analysis signal. You also have the ability to change between different modes of analysis.

To get you started, here are some ideas for how to use Expert Mode:
Use the filters to remove noise from your analysis signal. You can remove clicks and pops from your analysis signal to make sure that they don’t open the gate at the wrong moments.
Control an uneven stereo signal by applying separate gain to each channel or setting Analysis Mode to “Average”.
Create a mix of your main input and external sidechain input. Balance these correctly to create unusual gating polyrhythms.
For even more unusual gating behavior, change the analysis mode to “Average” and use two very different input sources.
