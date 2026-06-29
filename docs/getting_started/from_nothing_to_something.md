---
title: From Nothing to Something
parent: Getting Started
layout: default
nav_order: 10
authors:
  - key: fioh
    role: "Guide-Writer"
  - key: kaj
    role: "Editing"
---

# From Nothing to Something
How to go from having nothing, to getting your tools set up and having your character rigged and looking pretty in Blender.

In this section, we assume that you have NOTHING but a computer, internet, and motivation. We will go through the steps of:
- Having Nothing
- Having the correct programs and tools installed on them along with having a character in Blender, rigged and ready for you to animate.

Sounds like a dream, huh? Well then, let's get start with downloading what you need!

### FINAL FANTASY XIV
A bit of a no-brainer to start. Make sure that you have the game installed and that you are able to log-in! Have your username and password ready to enter into another log-in tool!

### XIVLAUNCHER
An alternate FFXIV launcher that is used to set up your in-game tools! It also helps you with logging in way faster too! 

Go to this website and follow the instructions for installation: [XIVLauncher Installation Guide](https://goatcorp.github.io/)

### BLENDER
Blender is a free 3D software that we use for FFXIV animations! It is built as a sort of "jack-of-all-trades". 3D animation is not just about the "animation", you may consider changing textures, making effects, compositing, tweaking character models and more! Blender CAN do it all very competently, however there may be far better choices for specific things!

Download the latest version of Blender here: [Blender Download](https://www.blender.org/download/)  
Alternatively you could use [Blender Launcher](https://victor-ix.github.io/Blender-Launcher-V2/) for an easier way to manage and update multiple Blender versions

NOTE: If Blender was RECENTLY updated, then the other tools *may* not have updated to catch up to the new version yet! If you suspect to have these issues, please contact the Mentors in the Discord server for the status.

---

## Checkpoint
Once you get to this point, open up FF14 using the XIVLauncher and open Blender just to see if it works! In-game, you should see Dalamud installed at the top left of the title screen.

![](assets/Blender_Example.png)
![](assets/Dalamud_Ok.png)

Once you have confirmed that both are downloaded and working, let's move on!

---

### MEDDLE
Meddle is the ONE in-game tool you need to get your character, weapons, items and environments from the game! It doesn't change gameplay or appearance of characters, all it does is copy the model it sees in the game, and extracts them into a format you can import into Blender!

You install Meddle through Dalamud, which appears when you start the game via the XIVLauncher! 

Follow the instructions here to install Meddle! [Meddle Website and Installation Guide](https://github.com/PassiveModding/Meddle)

Once you have the plug-in enabled in your game. You can go ahead and open it up! 
You should see a menu like so:

![](assets/Meddle_Instructions.png)

Ensure your character (or another character if you wish!) is selected in the dropdown menu, and hit `Export All Models`.
Ensure that you also export all additional file types, just so you have them! They will be used for an optional add-on later to make your equipment look really neat! 

Make sure you export it to a location you can find easily!

Note: Weapons are exported separately, below the character section, unless you click `Export All Models With Attaches`.

<br>

{: .important }
A lot of the required Blender add-ons can be installed via the [FFXIV Blender Plugins Master Repository](https://github.com/ShinoMythmaker/FFXIV-Blender-Plugins). It's recommended to use this method rather than individual installs you'll see below, simply because it's easier. In the end, all that matters is *that* you install them, not *how* you install them.

### AETHERBLEND
AetherBlend is a BLENDER add-on that you will use to import the files you exported from the game via Meddle!

Open Blender and follow instructions here to install AetherBlend: [AetherBlend Installation Guide](https://github.com/ShinoMythmaker/Aetherblend/wiki/Installation)

Note: It is mentioned in the instructions, but ensure that Rigify (an add-on that is INCLUDED in Blender) is also enabled!

### MEDDLE TOOLS
Meddle Tools is the BLENDER add-on that you will use to import things OTHER than characters! Monsters, Environment, Items etc. But even if you plan on only importing characters, AetherBlend requires Meddle Tools to be installed.

Open Blender and follow instructions here to install Meddle Tools: [Meddle Tools Installation Guide](https://github.com/PassiveModding/MeddleTools)

---

## Final Push
Now you have all you need to get started with importing your character! How does it all work?

Now, in Blender, create a new project. Delete the default cube by left clicking it and pressing "X".

With your cursor hovering over the 3D Viewport (the main work window), hit the "N" Key to open up the menu to the right!

You should see a menu like so. Navigate to the "AetherBlend" menu as shown here. Select `Import Character` and select the .gltf file you just exported from the game!

![](assets/Aetherblend_Setup.png)

Now you should see your character in-scene, with all the fundamental bones there, already selected in orange!

With the bones selected: click `Generate Rig` in the AetherBlend Menu.

![](assets/Generate_Rig.png)

This will create the actual rig you will use for posing!

![](assets/Final_Aetherblend.png)

After the rig is generated, Blender should default to "Pose Mode", which enables you to pose the rig you have selected. You can show/hide groups of bones to the right. 

Click on this button to enable the colored view mode!

![](assets/Textured_View.png)

You now, in essence, have a full on character model ready for you to start posing!

Now, you just have to learn how to do it!

As for questions like:

- "How do I actually move the parts of the model?" 
- "How do I show the colors of the model?" 
- "How do I create other objects and manipulate them?"
- "How do I begin animating?" & more? 

Well, now we are getting into "How to use Blender"!
That is what this next section, "Blender Basics" will cover!

Bringing a character to life is what the animation art form is all about! With study and practice,  you'll be having your character go from this:

![](assets/Fioh_A_Pose.png)

to this!

<video width="100%" height="auto" controls>
  <source src="assets/Fioh_Character_Select.mp4" type="video/mp4">
</video>

If you're brand new to Blender, continue on to [Blender Basics](blender_basics)!