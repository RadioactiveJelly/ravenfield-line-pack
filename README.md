# Ravenfield: Line Packs
-----

This is a quick rundown of how line packs work for the Community Based Text Chat mod.

# Requirements
1. **Unity 2020.3.48f1**
2. The latest version of the RF2020 Toolspack, found on the official RF discord.
3. Sourcetree (optional, but can make things easier for you if you clone the repo instead of just downloading the files)

# Setting Up
The first thing you should be taking a look at is the BaseLinePack prefab. **DO NOT EDIT ANYTHING ON THIS PREFAB**. It's important to keep this prefab untouched as edits directly to it may cause bugs. To make your own line pack, simply create a **variant of this prefab**.

Once you've made your variant, you'll notice the data containers already set up for you. Each data container has descriptions on when the lines they contain play so I won't repeat them here.

Next thing you need to make is your Content Mod prefab. First, make an empty object in your scene. Next, create an entry in the mutators array and add your line pack prefab to the entries Mutator Prefab field. Make sure to add a name, description and thumbnail as well. Do note, the prefab's name will be the name of your .rfc file when exported.

# Adding Lines
To add lines, all you need to do is add them in the array of strings in each data container. **IMPORTANT:** In the string array, each line's ID must be in the format of "lineX" with X being its place in the string array. See the sample lines already on the base pack. It's fine to leave a data container empty.

# Publishing
All done with setting up? Before you publish your mod, make sure to test it first! Select your content mod, and press Ctrl + E. This will export your mod. Now run the game with the Community Based Text chat mutator active and see if your lines are displaying properly. All good? Now go back to Unity and go to Ravenfield Tools -> Publish To Steam Workshop and follow the instructions there. 
