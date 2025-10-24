# HSVoiceCommandVR


This mod is for incorporating many Voice Commands in MainGame/StudioNEO (some functions are restricted in MainGame). 
Many actions, face/hand/body expressions or operations get able to be invoked by real voices (or voice pannel on GUI).


## [Installation]
1. Install HoneySelect VRmod with LRE & IBL (full pack) version 1.7 or more.
2. On ${GameFolder}/vr_settings_for_IBL.xml, set "true" at \<SpeechRecognition\> item and already installed appropriate Language Pack name at \<Locale\> item (for example, en-US, ja-JP etc.).
3. Run (HoneySelect|StudioNEO)_(64|32)_for_VR_with_IBL.
4. Enjoy super high quality on VR!

**Caution!** 
- For using Voice Commands by real voices, you should install at least one Speech recognition Language Pack (having recognition engine) in Windows and enable microphone function of your PC.
- For installing Speech recognition Language Pack in Windows, please refer to   
[Installing New Languages | Text or Speech to Text | Windows 11 https://www.youtube.com/watch?v=lKMFbOEcT-E]. 
- Which Speech recognition Language Packs you have already installed or what you have set as \<Locale\> item are able to be checked via ${GameFolder}\UserData\dictionaries\Please_check_used_speech_recognition_engine.txt.
- If you dont install Speech recognition Language Pack at all, you can use only voice pannel on GUI (not real voices).
- Each Language Pack dictionary (for example, en-US.txt, ja-JP.txt etc.) will be created automatically at first if not existing at all in ${GameFolder}\UserData\dictionaries\\. 
- On each Language Pack dictionary (for example, en-US.txt, ja-JP.txt etc.), you can add/remove/change your favorite voice pronunciations as a row for each voice command.
- Each voice pronunciation for each voice command in each Language Pack dictionary is distinguished by prefixes (or prefix word) from other voice pronunciations. Plese don't add/change voice pronunciation with same prefixs (or prefix word) as others.  

## [Requirements]
- Game updated with the last patch and DLC installed
- Installed and set up SteamVR
- HoneySelect VRmod with LRE & IBL (full pack) version 1.7 or more.
- At least one Speech recognition Language Pack installed already in Windows.

## [Uninstall]
- On ${GameFolder}\vr_settings_for_IBL.xml, set "false" at \<SpeechRecognition\> item.
Or remove some installed DLL in (${GameFolder}\Plugins\). Ones to remove are as below,  
-- VR\SpeechServer.dll
-- VR\SpeechTransport.dll
-- VR\NAudio.dll
  
## [Setting files]
- General setting:  
  -- ${GameFolder}\vr_settings_for_IBL.xml   --- each settings for Speech Recognition  
- Dictionaries:  
  -- ${GameFolder}\UserData\dictionaries\Please_check_used_speech_recognition_engine.txt     --- result of checking already installed Speech recognition Language Packs and used Language Pack  
  -- ${GameFolder}\UserData\dictionaries\en-US.txt    --- voice commands dictionary for en-US Language Pack (default)  


## UI/UX abstract on HSVoiceCommandVR
Tag      |  Move   | 
----     | ------  | 
no hand needed
<kbd>indicated voice (or voice pannel)</kbd> | apply indicated action for one possible human chara seen by you in current scene
only one hand needed
<kbd>menu + holding + indicated voice (or voice pannel)</kbd> | apply indicated action for all human charas in current scene



## Voice commands and pronunciations
List below is from en-US.txt (default). On your indicated Speech recognition Language Pack, your favorite pronunciations can be added/removed/changed as a row.
Speech Recognition engine distinguishes each pronunciation by prefixes (or prefix word).

| Voice Command        | Pronunciations       | Explanation |
| ----------- | ------------------- | -----|
| Seated      | This mode lets you play the game with a mouse, keyboard, or gamepad.<br />The controls are essentially the same as in the main game. The screen is presented on a big monitor in front of you. |
| Standing    | *Default mode.* As soon as tracked controllers are registered by the game, it switches into *standing mode*, also called *room scale mode*. In this mode, you can freely move around and use your Vive or Touch controllers to stuff. |


