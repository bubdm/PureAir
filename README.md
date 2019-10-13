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

# About

The PureAir Engine is the successor to my previous, "Titus's Triple Bypass Valve" Expression 2. PureAir is an Expression 2 that interfaces with [RLCPT Gamma](https://github.com/MagnumMacKivler/RLCPT2) and it's corresponding Control Reader E2. 

PureAir Engine uses the pre-calculated (from the Gamma Chip) air brake pressure(s), brake pipe volume, and Air Flow in Cubic Feet per Minute (CFM) to calculate air brake application and releasing sound(s), duration(s), volume and pitch. Ordinary RLC Gamma uses a predefined application and release sound, which if you had a long string of rollingstock behind the lead locomotive, the apply (and or release) sounds would not change (stay the same), if you had a smaller string of cars, hence, non-responsive. 

The PureAir Engine calculates the length of the train, and uses the air pressure and air flow rate to determine how long to play the application sound, how loud (volume) and then pitch (depending on situation), this also applies for releasing or any other changes between. PureAir simulates distribution valves and air leakage, furthermore adding to the realism. PureAir takes a responsive approach towards how it calculates the sound parameters, any and every aspect of the locomotives braking system and the trains braking system is taken into account, providing the most realistic experience for the driver. 

We are constantly updating the engine for better simulation, and for varying engines and setups. With the HTTPS version checking system you can make sure you have the latest version with the best performance. Each release is rigorously tested before being published, to make sure of absolute quality, and to get rid of any bugs. PureAir Engine is made for developers, with the new Extensions folder for user made mods, expanding the possibilities, which are endless.

We are always trying to improve our products for the best user experience possible, if you would like to request a feature or report a bug or glitch you found while using the PureAir Engine, or just a question, post it on the GitHub Issues Tab.


# Release Types

* **Current**: Not Under active development. Finished and polished (but may still contain minor bugs) versions of the code Release. (for example, **Version 2.x.x (Current)**).
* **Betas**: Under active development. Code in the Beta release(s) is currently being worked on, it may contrain game breaking bugs. (for example, **Version 2.x.x (Beta)**).
* **LTS**: Releases that receive Long-term Support, with a focus on stability. Note if you use an LTS release you may encounter compatibility issues with newer (or older) versions depending on the code version. (for example, **Version 2.x.x (LTS)*
* **Misc**: Miscellaneous Release. Reasoning for release will be explained in the Release Description. (for example, **Version 2.x.x (Misc)**).

Current, Betas, LTS and Misc releases follow [Semantic Versioning](https://semver.org). A
member of the Release Team signs each Current, Beta, LTS, and Misc release.

# Installation

To install the PureAir Engine on a locomotive is fairly straight forward. You will need a basic understanding of Experssion 2, Wiremod, and Garry's Mod in general.


### Required Addons

| NOTE | You will also need "Titus's Locomotive Propper Model Pack 2.4" Addon for the PureAir Engine to work correctly. |
| :--- | :--- |

Titus's Locomotive Propper Model Pack 2.4: https://steamcommunity.com/sharedfiles/filedetails/?id=1809527658


### Download the PureAir Engine

**1.** Head to the releases tab of the PureAir GitHub

<p align="left">
  <a href="https://titusstudios.net/data/static/images/rlcpt2_readmeimg5.jpg">
    <img
      alt="pureair-engine"
      src="https://titusstudios.net/data/static/images/rlcpt2_readmeimg5.jpg"
    />
  </a>
</p>

**2.** Download the Release of your choice (usually the latest one), usually you will only be downloading `(Current)` Releases.

<p align="left">
  <a href="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2000-48-02.png">
    <img
      alt="pureair-engine"
      src="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2000-48-02.png"
    />
  </a>
</p>

| NOTE | Download by clicking the `Source code (zip)` button. |
| :--- | :--- |

**3.** Open the Zip file using a program like WinZip or WinRar, if it didn't open automatically. Then open the first folder in the zip file. **DO NOT** Extract the first folder (Ex, `PureAir-x.x.x`)! E2 will not work correctly! 


<p align="left">
  <a href="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2000-48-54.png">
    <img
      alt="pureair-engine"
      src="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2000-48-54.png"
    />
  </a>
</p>

<p align="left">
  <a href="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2000-49-01.png">
    <img
      alt="pureair-engine"
      src="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2000-49-01.png"
    />
  </a>
</p>

| CAUTION | You want to see the folder seen above (ex, `pureair-engine`, if you dont, you are not in the right location and after extracting the E2 will not function. |
| :--- | :--- |

**4.** Extract the `pureair-engine` folder directly into: `<Your active steam directory>\SteamApps\common\Garry's Mod\garrysmod\data\expression2\`.
The file path should then look like `..\expression2\pureair-engine\..`.

| CAUTION | If you see the folder `PureAir-x.x.x` inside the `expression2` folder, YOU INSTALLED IT WRONG! ...and the E2 will not work! Follow the install guide again. |
| :--- | :--- |

| NOTE | If you're currently in-game in Garry's Mod, open the E2 Editor, and click the "Update" button under the list of E2s on the lefthand side of the window. |
| :--- | :--- |


### In-Game Setup

#### Inital Setup
1. Spawn the Engine Processor (`titus's_pureair_engine_processor`)
2. Place the E2 somewhere on the locomotive, usually next to the RLC chip, or other chips. 
3. Multiparent the E2 to the Locomotive Body, or a parenting Gate.
4. Get the Wiremod Wiring tool out, and look at the PureAir Engine Processor.

#### Wiring (Part A - Control Stand Editing)
The PureAir Engine needs to know if and when you apply, release or move the Automatic Brakes. Sadly as PT Gamma doesnt have a direct output for it, we have to edit the RLCPT Gamma Control Stand E2 slightly.

1. Find the Control Stand E2, This will be one of the following ( Expression 2(s) ):
* cstand_aar
* cstand_emd_composite
* cstand_ge_kc92
* cstand_sd60m_desktop
2. Open the E2 with the Expression 2 tool.
3. In the Control Stand E2, add the following to the output lines; `IncreaseTrainBrake` and `DecreaseTrainBrake`.
These are what the following changes should look like:

**Before:**
<p align="left">
  <a href="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2001-26-46.png">
    <img
      alt="pureair-engine"
      src="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2001-26-46.png"
    />
  </a>
</p>

**After:**
<p align="left">
  <a href="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2001-27-17.png">
    <img
      alt="pureair-engine"
      src="https://titusstudios.net/data/static/images/pureair-engine/Screenshot%20from%202019-10-13%2001-27-17.png"
    />
  </a>
</p>

| NOTE | This edit to the control stand chip works with any version (for PT Gamma), newer and older versions will work with this edit. |
| :--- | :--- |

4. Save and Exit the Control Stand E2


#### Wiring (Part B - Wiring PureAir Inputs)
1. Wire `IncreaseTrainBrake` to the Control Stand E2s `IncreaseTrainBrake` Output.
2. Wire `DecreaseTrainBrake` to the Control Stand E2s `DecreaseTrainBrake` Output.
2. Wire `EqualRes` to the RLCPT Gamma Chip's `EqualRes` Output.
2. Wire `CFM` to the RLCPT Gamma Chip's `CFM` Output.
2. Wire `LocoBrakePressure` to the RLCPT Gamma Chip's `LocoBrakePressure` Output.
2. Wire `BrakeCutIn` to your Automatic Brake Cut-In Button.
2. Wire `AirBrakeMode` to the RLCPT Gamma Chip's `AirBrakeMode` Output.
2. Wire `LOCOMOTIVE_ENTITY` to the Locomotive Body.

| NOTE | The `LOCOMOTIVE_ENTITY` is an optional input. If it is not wired, the sound will emit from the E2 origin, and not the Locomotives Models origin. |
| :--- | :--- |

#### Final Setup
To Complete the setup of the PureAir Engine, you will need to remove the normal air braking sounds from the Control Stand E2. The following strings should look like this for proper operation.

```csharp

AirBrakeApply = ""
AirBrakeRelease = ""

LocoBrakeFull = ""
LocoBrakeReleaseSoft = ""
LocoBrakeReleaseHard = ""

```

| NOTE | Any strings not shown above can be set to the default or to your liking. |
| :--- | :--- |


# File Structure

* [_root](#_root)
  * [pureair-engine](#pureair-engine)
    * [config](#config)
      * `defaultengine.txt`
    * [extensions](#extensions)
    * [resources](#resources)
      * `entity-selection.txt`
    * [scripts](#scripts)
      * `delta-dampening.txt`
      * `localprint.txt`
      * `localsound.txt`
    * [workers](#workers)
      * `https-beginrequest-worker.txt`
      * `https-version-worker.txt`
      * `https-worker.txt`
    * `titus's_pureair_engine_processor.txt`

***

### _root
Root directory, most cases will be: `../data/expression2/`

### pureair-engine
PureAir Engine's main directory, all files reguarding the Engine are stored in here.

### Config
PureAir Engine config files. Contains engine config, defaults, etc.

### Extensions
PureAir Engine Extensions. User made addons (for the engine) will be added here, and accessed by the processor here.

### Resources
PureAir Engine Resources. Contains any; scripts, assets, lua, etc... that is used for getting info outside of the engine itself. Such as; BrightStar connection, RLCPT Gamma interface, sound emission entity source, etc.

### Scripts
All scripts for the main processor. Mostly used for external functions, for modification.

### Workers
Worker scripts. Pretty much everything to do with HTTP and HTTPS requests. Handles all requests for data on the internet.

***


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

The PureAir Engine also has default engine settings, these can be found at `../pureair-engine/config/defaultengine.txt`

### Default Engine Settings
```csharp

E = entity()
O = owner()

SILENT = 0
DEBUG = 0

```

| NOTE | Editing the default sound, engine, or other script settings may cause unexpected results, preformance issues, or possible stability issues. |
| :--- | :--- |

