# HSVoiceCommandVR


This mod is for incorporating many Voice Commands in MainGame/StudioNEO (some functions are restricted in MainGame). 
Many actions, face/hand/body expressions or operations get able to be invoked by real voices (or voice panel on GUI).


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
- If you dont install Speech recognition Language Pack at all, you can use only voice panel on GUI (not real voices).
- Each Language Pack dictionary (for example, en-US.txt, ja-JP.txt etc.) will be created automatically at first if not existing at all in ${GameFolder}\UserData\dictionaries\\. 
- On each Language Pack dictionary (for example, en-US.txt, ja-JP.txt etc.), you can add/remove/change your favorite voice pronunciations as a row for each voice command.  
![Image](https://github.com/user-attachments/assets/911bbd4d-5fc9-44f8-ad6d-4075795bbc81)  

- Each voice pronunciation for each voice command in each Language Pack dictionary is distinguished by prefixes (or prefix word) from other voice pronunciations. Plese don't add/change voice pronunciation with same prefixs (or prefix word) as others.  
For example, if you register "look" for one voice command and "look at me" for other voice command then you pronounce "look at me", both voice commands are invoked so this setting undesirable.  
Or as another example, if you register "walk very near" for one voice command and "walk very far" for other voice command then you pronounce "walk very far", only voice command of "walk very far" is invoked so this OK.
- On Sex Motions by voice command, appropriate sex motion (random) is invoked by where the height-position of your headset in game is against the height-position of chara's hip.
For example, height-position of your headset in game is about at height-position of chara's face, hip or foot, by respective situation invoked sex motion would be different.  

## [Requirements]
- Game updated with the last patch and DLC installed
- Installed and set up SteamVR
- HoneySelect VRmod with LRE & IBL (full pack) version 1.7 or more.
- At least one Speech recognition Language Pack installed already in Windows.

## [Uninstall]
On \\{GameFolder}\vr_settings_for_IBL.xml, set "false" at \<SpeechRecognition\> item.
Or remove some installed DLL in (\\{GameFolder}\Plugins\). Ones to remove are as below,  
- VR\SpeechServer.dll
- VR\SpeechTransport.dll
- VR\NAudio.dll
  
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
<kbd>indicated voice (or voice panel)</kbd> | apply indicated action for one possible human chara seen by you in current scene
only one hand needed
<kbd>menu + holding + indicated voice (or voice panel)</kbd> | apply indicated action for all human charas in current scene



## Voice commands and pronunciations
List below is from en-US.txt (default). On your indicated Speech recognition Language Pack, your favorite pronunciations can be added/removed/changed as a row.
Speech Recognition engine distinguishes each pronunciation by prefixes (or prefix word).

| Voice Command        | Pronunciations       | Explanation |
| ----------- | ------------------- | -----|
\< /// MainGame & Studio common commands /// \>
| Impersonate    | impersonate    | Move and Impersonate seen chara                  |         
| LoadSettings   | load settings  | Load current settings of vr_settings_for_IBL.xml |
| ResetSettings  | reset settings | Set default values of vr_settings_for_IBL.xml    |
| IncreaseScale  | increase scale | Increase IPD                                     |
| DecreaseScale  | decrease scale | Decrease IPD                                     |
| IBL            | ibl, test      | IBL GUI on/off                                   |
| HSSSS          | hsss           | HSSSS config GUI on/off                          |
| Debug          | debug          | Debug console GUI on/off                         |
| VoicePanel     | voice panel    | This Voice Panel on/off                          |
\< /// only Studio commands below /// \>
\< /// Move /// \>
|ComeOnWalk| come on walk  | Come walking up to me  |
|ComeOnRun | come on run   | Come running up to me  |            
|FrontOfMe | front of me   | Come in front of me    |
|CloseToMe | close to me   | Come just close to me  |
|NextToMe  | next to me    | Come next to me        |
|FollowMe  | follow me     | Follow me              |
\< /// Sex /// \>
|ComeOnKiss| come on kiss |  Come and Kiss             |
|SexNormal | sex normal   |  Come and Normal Sex       |
|SexBack   | sex back     |  Come and Back Sex         |
|OralSex   | oral sex     |  Come and Oral Sex         |
|Cowgirl   | cowgirl      |  Come and Cowgirl Sex      |
|Handjob   | handjob      |  Come and Handjob Sex      |
|BreastSex | breast sex   | Come and Breast Sex        |
|Masturbation  | masturbation  | Masturbation              |
|TwoMenSex     | two men sex   | Two Men Sex               |
|TwoWomenSex   | two women sex | Two Women Sex             |
|Shower        | shower        | Shower                    |
|Toilet        | toilet        | Toilet                    |
|VariousSex    | various sex   | Various Sex               |
|SpeedNormal      | speed normal   | Animation Speed Normal              |
|SpeedZero        | speed zero     | Animation Speed Zero                |
|SpeedMax         | speed max      | Animation Speed Max                 |
|SpeedUp          | speed up       | Animation Speed Up                  |
|SpeedDown        | speed down     | Animation Speed Down                |
|PatternNormal    | pattern normal | Animation Pattern Normal            |
|PatternMinus     | pattern minus  | Animation Pattern value Minus One   |
|PatternPlus      | pattern plus   | Animation Pattern value Plus One    |
|PatternUp        | pattern up     | Animation Pattern value Up          |
|PatternDown      | pattern down   | Animation Pattern value Down        |
|CategoryUp       | category up    | Motion: Category Number Up          |
|CategoryDown     | category down  | Motion: Category Number Down        |
|AnimationUp      | animation up   | Motion: Animation Number Up         |
|AnimationDown    | animation down | Motion: Animation Number Down       |
\< /// Look /// \>
| LookStraight    | look straight   | Eye & Neck straight                |  
| LookAtMe        | look at me      | Eye & Neck to me                   |  
| LookNeckAtMe    | look neck at me | Only Neck to me                    |  
| LookAnime       | look anime      | Only Neck Anime                    |  
| LookFix         | look fix        | Eye & Neck fix                     |  
| LookNeckFix     | look neck fix   | Only Neck fix                      |  
| LookEyeFix      | look eye fix    | Only Eye fix                       |  
| LookAway        | look away       | Only Eye look away                 |  
| LookManipulate  | look manipulate | Only Eye Manipulation              |  
\< /// Face /// \>            
| FaceNormal      | face normal     | Eye & Mouth default(0)             |  
| EyeUp           | eye up          | Only Eye Number Up                 |  
| EyeDown         | eye down        | Only Eye Number Down               |  
| EyeOpen         | eye open        | Only Eye Opent                     |  
| EyeClose        | eye close       | Only Eye Close                     |  
| EyeHalf         | eye half        | Only Eye Half                      |  
| MouthUp         | mouth up        | Mouth Number Up                    |  
| MouthDown       | mouth down      | Mouth Number Down                  |  
| MouthOpen       | mouth open      | Mouth Open                         |  
| MouthClose      | mouth close     | Mouth Close                        |  
| MouthHalf       | mouth half      | Mouth Half                         |  
| Kiss            | kiss            | Eye & Mouth Kiss                   |  
| Tongue          | tongue          | Eye & Mouth Tongue                 |  
\< /// Hand /// \>            
| HandNormal      | hand normal     | Both Hand default(0)               |  
| HandBothUp      | hand both up    | Both Hand Number Up                |  
| HandBothDown    | hand both down  | Both Hand Number Down              |  
| HandLeftUp      | hand left up    | Left Hand Number Up                |  
| HandLeftDown    | hand left down  | Left Hand Number Down              |  
| HandRightUp     | hand right up   | Right Hand Number Up               |  
| HandRightDown   | hand right down | Right Hand Number Down             |  
\< /// MMD /// \>
| MMDOn           | mmd on          | MikuMiku Dance On during MMD       |  
| MMDOff          | mmd off         | MikuMiku Dance Off during MMD      |  
\< /// Accessory /// \>
| ChangeCostume   | change costume  | Change Costume                     | 
| ChangeNaked     | change naked    | Change Naked Status                |  
| ChangeAccessory | change accessory| Change Accessory Status            |  
| SelectVoice     | select voice    | Voice Panel Shown                  | 
| ChangeSiru      | change fluid    | Change Fluid Status                |  
| ChangeTears     | change tears    | Change Tears Status                |  
\< /// Some Dances /// \>            
| PoleDance       | pole dance      | Pole Dance                         |  
| DefaultDance    | default dance   | Some Dances                        |  
\< /// End Tool /// \>     
| NotShown        | deselect        | Not Show Game Panel                |  
| Stop            | stop            | Stop All Motion                    |  
        

