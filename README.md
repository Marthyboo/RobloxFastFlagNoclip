> **Fast Flags are extremely powerful, being that they are intended to only be used by Roblox engineers. While they can be very useful, they can cause issues with stability and functionality if you don't know what you're doing.**

## Bloxstrap How to Use:
1. **Open the [Bloxstrap Menu](https://github.com/pizzaboxer/bloxstrap).**
2. **Navigate to `Fast Flags` >> `Fast Flags Editor` >> `Add New` >>  `Import Json`.**
3. **Paste in the JSON.**
4. **Save and your good to go!**

<img src="/assets/tutorial260.gif" width="750"/>

# The Noclip Below no longer works, However There is an alternative, But it sucks as an alternative. 

```
{ "FIntPGSPenetrationMarginMax": "2147483647",
 "FIntPGSPenetrationMarginMin": "2147483647",
"DFIntAssemblyExtentsExpansionStudHundredth": "-50" }
```
- FIntPGSPenetrationMarginMax ("2147483647"): the maximum penetration margin between objects, effectively removing any limit with maximum int number
- FIntPGSPenetrationMarginMin ("2147483647"):  almost the same thing, the minimum penetration margin, but instead keeps objects from being too close
- The main noclip, DFIntAssemblyExtentsExpansionStudHundredth ("-50"): adjusts the extent of an object like a wall, modified with a negative value





###  Better NoClip Modified [Patched]
```
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntMaximumFreefallMoveTimeInTenths": "1000",
    "DFIntDebugSimPrimalStiffness": "5"
}
```

dfintdebugsimprimalstiffness: "1" is the main part of the noclip. by default, its 0, but at that level, objects can fall through the floor, which you've probably seen in games. set it to 1 or higher (like 10) to fix that, though higher values make objects move through walls slower. a good range is around 1-5 or 5-7 for a balance.

also incase you don't understand how this even works, DFIntDebugSimPrimalStiffness setting controls how stiff objects are in the simulation. a value of 0 means objects are very flexible and easy to bend or deform.


###  NoClip For Car Games [Patched]
the other noclip makes cars fall like quicksand no matter what, so just use this for any games with cars
```
{
  "DFIntAssemblyExtentsExpansionStudHundredth": "-50",
  "FIntPGSPenetrationMarginMax": "2147483647",
  "DFIntMaximumFreefallMoveTimeInTenths": "1000",
  "FFlagDebugSimDefaultPrimalSolver": "True",
  "FIntPGSPenetrationMarginMin": "2147483647"
}
``` 
