<p align="center">
  <a href="https://www.titusstudios.net/">
    <img
      alt="pureair-engine"
      title="www.titusstudios.net/"
      src="https://titusstudios.net/data/static/images/pureair-engine/og-image2.png"
      width="400"
    />
  </a>
</p>

<br>


PureAir Engine is an environment responsive air braking processor built on Wiremod's Expression 2 Environment.


# Defaults and Settings

The PureAir Engine, depending on the appilcation, has default sound settings which are siffcant in most cases. If however, you would like to change the preset defaults...

Navigate to `../pureair-engine/titus's_pureair_engine_processor.txt` and open the main processor using the in-game editor or [Microsoft Visual Studio Code](https://code.visualstudio.com/)

| NOTE | If you are using Visual Studio Code, set the plain text file(s) workspace to `C#` / `CSharp` or, download the [Expression 2 Workspace Extension](https://github.com/DjHaski/VSCode-E2) for Visual Studio Code |
| :--- | :--- |

The Default Sound Path and Sound Pitch settings are located under the Include Library

### Default Sound Settings:
```csharp

# SETTINGS

Automatic_application = "titus's_locomotive_propper_model_pack_2.4/loops/s_nippongallery_trainapplicationfull.wav"
Automatic_release_whine_FEATURE = 0
Automatic_release_whine = "titus's_locomotive_propper_model_pack_2.4/loops/s_nippongallery_brakereleasehisswhine.wav"
Automatic_release_flow = "titus's_locomotive_propper_model_pack_2.4/loops/s_f40ph_servicerelease.wav"

Independant_MasterPitch = 105
Independant_application = "titus's_locomotive_propper_model_pack_2.4/loops/s_nippongalleryserviceloop2.wav"
Independant_flow = "titus's_locomotive_propper_model_pack_2.4/loops/s_nippongallery_servicerelease.wav"

```

| NOTE | Editing the default sound, engine, or other script settings may cause unexpected results, preformance issues, or possible stability issues. |
| :--- | :--- |

