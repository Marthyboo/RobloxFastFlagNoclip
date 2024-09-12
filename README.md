> **Fast Flags are extremely powerful, being that they are intended to only be used by Roblox engineers. While they can be very useful, they can cause issues with stability and functionality if you don't know what you're doing.**

## Bloxstrap How to Use:
1. **Open the [Bloxstrap Menu](https://github.com/pizzaboxer/bloxstrap).**
2. **Navigate to `Fast Flags` >> `Fast Flags Editor` >> `Add New` >>  `Import Json`.**
3. **Paste in the JSON.**
4. **Save and your good to go!**

<img src="/assets/tutorial260.gif" width="750"/>

## Normal Roblox Bootstrapper How to Use:
###### You can also do Roblox Studio
1. **Navigate to your Roblox Installation directory. Typically found at `%localappdata%\Roblox\Versions\` or `C:\Program Files (x86)\Roblox\Versions`.**
2. **Identify the folder `version-xxxxxxxxxxxxxxxx` ~~containing `RobloxPlayerBeta.exe`~~ You can do this for Roblox Studio too.**
3. **Create a new folder named `ClientSettings`. Inside this folder, place the file `ClientAppSettings.json`.**
4. **Paste the JSON into `ClientAppSettings.json`. (You can utilize ChatGPT to format multiple JSONs for clarity if needed)**
5. **Save and you're good to go!**
###### Do note that after roblox updates you have to do this process again

[Watch a Video Tutorial](https://streamable.com/rk5an6)

###  Better NoClip Modified
```
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntMaximumFreefallMoveTimeInTenths": "1000",
    "DFIntDebugSimPrimalStiffness": "5"
}
```

dfintdebugsimprimalstiffness: "1" is the main part of the noclip. by default, its 0, but at that level, objects can fall through the floor, which you've probably seen in games. set it to 1 or higher (like 10) to fix that, though higher values make objects move through walls slower. a good range is around 1-5 or 5-7 for a balance.

also incase you don't understand how this even works, DFIntDebugSimPrimalStiffness setting controls how stiff objects are in the simulation. a value of 0 means objects are very flexible and easy to bend or deform.

