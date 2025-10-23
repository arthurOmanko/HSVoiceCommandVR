# HSVoiceCommandVR


This mod is for incorporating many Voice Commands in MainGame/StudioNEO. (some functions are restricted in MainGame)
Many actions, face/hand/body expressions or operations get able to be invoked by real voices (or voice pannel on GUI).


## [Installation]
1. Install HoneySelect VRmod with LRE & IBL (full pack) version 1.7 or more.
2. On ${GameFolder}/vr_settings_for_IBL.xml, set "true" at \<SpeechRecognition\> item and already installed appropriate Language Pack name at <Locale> item (for example, en-US, ja-JP etc.).
3. Run (HoneySelect|StudioNEO)_(64|32)_for_VR_with_IBL.
4. Enjoy super high quality on VR!

**Caution!** 
- For using Voice Commands by real voices, you should install at least one Speech recognition Language Pack in Windows.
- Which Speech recognition Language Packs you have already installed or what you have set as <Locale> item are able to be checked via ${GameFolder}\UserData\dictionaries\Please_check_used_speech_recognition_engine.txt.
- If you dont install Speech recognition Language Pack at all, you can use only voice pannel on GUI (not real voices).

## [Requirements]
- Game updated with the last patch and DLC installed
- Installed and set up SteamVR
- HoneySelect VRmod with LRE & IBL (full pack) version 1.7 or more.
- At least one Speech recognition Language Pack installed already in Windows.

## [Uninstall]
On ${GameFolder}/vr_settings_for_IBL.xml, set "false" at <SpeechRecognition> item.
Or remove some installed DLL in (${GameFolder}/Plugins/). Ones to remove are as below,  
- HSVoiceCommandVR.dll
- VR/SpeechServer.dll
- VR/SpeechTransport.dll
- VR/NAudio.dll
  
After it, if you want previous VR environment, for example, from VRmod by Eusth, install Eusth's VRmod Tool and rewrite some data by it. VR environment and related data by Eusth's VRmod can come back. 


## [Setting files]
- General setting:  
  -- ${GameFolder}\vr_settings_for_IBL.xml   --- each settings for Speech Recognition
- Dictionaries:  
  -- ${GameFolder}\UserData\dictionaries\Please_check_used_speech_recognition_engine.txt  --- Result of checking already installed Speech recognition Language Packs and used Language Pack
  -- ${GameFolder}\UserData\dictionaries\en-US.txt  --- voice commands dictionaries for en-US Language Pack (default)
  

## Modes & Controls

HoneySelectVR comes in two *modes*:

| Mode        | Description         |
| ----------- | ------------------- |
| Seated      | This mode lets you play the game with a mouse, keyboard, or gamepad.<br />The controls are essentially the same as in the main game. The screen is presented on a big monitor in front of you. |
| Standing    | *Default mode.* As soon as tracked controllers are registered by the game, it switches into *standing mode*, also called *room scale mode*. In this mode, you can freely move around and use your Vive or Touch controllers to stuff. |

### Common Mode
