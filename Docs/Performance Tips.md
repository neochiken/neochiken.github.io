---
title: Performance Tips
layout: home
nav_order: 3
---

# Performance Tips
There are a couple things you can do that can help with performance that I recommend.

## Using OpenComposite
To switch to Open Composite select OC swapper in the dropdown menu in MO2

![OCSwapper1](/assets/images/OCSwapper1.png)

then click the button!

![OCSwapper2](/assets/images/OCSwapper2.png)

Then you will need to set your prefered platform to handle OpenXR
***ONLY SET ONE NOT ALL THREE!***

![OpenXRSelect](/assets/images/OpenXRSelect.png)

Optionally if you would like to have a name other than Tahrovin when using Open Composite you can use the OC Character Renamer in the Your Choices section of MO2. Just right click on the mod, open in explorer, open the root folder and open opencomposite.ini. You can then change Tahrovin to be whatever you want your character to be named when you finish character creation.

![OCCharacterNamer](/assets/images/OCCharacterNamer.png)

## Profiles
There are three different profiles in Tahrovin, default which uses community shaders and reshade (Medium performance impact), ENB which uses ENB VR for visuals (High Performance impact), and then performance which only uses reshade and has the least performance impact.

## Skyrim Upscaler
If you have a 20xx or newer series Nvidia card I default skyrim Upscaler to DLAA for visuals, but you can change it from DLAA to DLSS to increase performance at the cost of some visual fidelity.



# Oculus and Oculus Link Specific Advice



## Change Refresh Rate
Changing the refresh rate to a higher one in the Oculus settings reduces the maximum resolution delivered to your headset as well as offering a smoother feel to the game. The reduced resolution will help the game run at a more stable FPS and likely a higher FPS. Combine the higher FPS with the higher refresh rate of the Quest 2 and you have a much nicer game playing experience. 

So, to do this you need to start by connecting your Quest 2 headset to your PC via USB, power your headset on and then head over to **Devices** in the left-hand menu of the Oculus PC client.

![Oculus Client 1](/assets/images/OculusClient00.jpg)

When in there, connect select the top menu option:

![Oculus Client 2](/assets/images/OculusClient01.png)

In the right-hand menu that pops-up, scroll down to **Graphics Preferences**:

![Oculus Client 3](/assets/images/OculusClient02.png)

In the pop-up menu, ensure that the **Automatic** resolution scaling is *OFF*. I recommend trying each setting in turn to see at which point you get the best look vs performance. I can't tell you what point that would be because it's a subjective choice. Also ensure that the **Rendering Resolution** is at *1.0x* as stated in the main readme.

![Oculus Client 4](/assets/images/OculusClient03.png)

Once you've made your changes, click **OK**.

## Increase the Oculus Link USB Data Rate
For some odd reason, the default Oculus Link settings limit the USB data rate between your PC and the Oculus headset to 100Mbps but the maximum link speed is **500Mbps.** That's *5 times* the data rate over the regular setting.

Increasing the USB data rate means that your PC and your headset can communicate much faster, meaning that VR games will look sharper because there is less compression needed on the data as well as a noticeable reduction in artifacts and flickering in your vision.

To do this, head to the installation folder of the Oculus PC client, usually `C:\Program Files\Oculus`, and head into the **Support** folder:

![Explorer 1](/assets/images/Explorer00.png)

Once there, head into the **oculus-diagnostics** folder:

![Explorer 2](/assets/images/Explorer01.png)

Once there, run the **OculusDebugTool**:

![Explorer 3](/assets/images/Explorer02.png)

in the Oculus Debug Tool, change **Encode Bitrate (Mbps)** to 350. You can go as high as 500Mbps as mentioned earlier but try somewhere in the middle first before going all in.

![Oculus Debug Tool 1](/assets/images/OculusDebugTool00.png)

Once changed, close out the tool and done!

## Monitoring Performance with an Oculus Quest 2
The Oculus Debug Tool also comes with a performance overlay. Follow the steps above to open the Oculus Debug Tool and set the **Visible HUB** option to *Performance*.

***DON'T CLOSE THE OCULUS DEBUG TOOL AS THIS WILL ALSO CLOSE THE PERFORMANCE OVERLAY.***

You will know when it is enabled as soon as you put on your headset. You can use the info here to help with monitor the performance you are getting in-game.