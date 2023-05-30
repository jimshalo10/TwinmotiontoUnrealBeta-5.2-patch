#TwinmotiontoUnrealBeta-5.2-patch

This patch is for the Twinmotion for Unreal 5.2 Epic binary when Downloaded from the Epic Games Launcher version 15.2 and above 

To check see in bottom of Launcher Settings page

Twinmotion Trial 2023.1.1 is available as of 30th May2023 at https://www.twinmotion.com/en-US/license

Exit Unreal 5.2 Epic binary before starting this procedure

To download this click the green dropdown marked "Code" above and select "2Download zip". DONT attempt to use Git clone it will fail!

This will produce a 554 MB zip file in your Download directory called 

"TwinmotiontoUnrealBeta-5.2-patch-TwinmotiontoUnrealBeta-5.2-patch.zip"

Navigate to your 5.2 binary distribution at "C:\Program Files\Epic Games\UE_5.2" or "D:\Program Files\Epic Games\UE_5.2" depending where you installed UE 5.2

Now open with the standard Windows10/11 Windows Explorer extractor by right clicking the zip file

Extract with a zip extractor, like WinRAR, or the Windows Explorer navigate to the "Engine" folder and extract.

In the "C:\Program Files\Epic Games\UE_5.2\Engine\Plugins" you should see the Plugin Directory "TwinmotiontoUnrealBeta"

If you do not see that the you need to check the way your zip extract was correct.

The installation and usage tutorial is available at 

https://dev.epicgames.com/community/learning/tutorials/K8nX/twinmotion-to-unreal-engine-5-1-5-2-for-virtual-camera-workflows

There are several inportant amendments to adding plugins below described in the tutorial section 10

Section 10 Once the Plugin window opens, enable the following plugins: 

The plugins can be added together, without restarting editor each time, from UE Editor navigate to "Edit ->Plugins"


1. Datasmith Importer
2. Dataprep Editor
3. Sun Position Calculator
4. Datasmith Twinmotion Content   version 2023.1

The version number must be 2023.1 not an earlier version or it will fail. Remove with procedure described in tutorial for earlier versions

There are only four plugins needed. The plugin "Twinmotion Content" does not exist.

All assets are now in "Engine/Plugins/TwinmotiontoUnrealBeta/Content/Twinmotion/"


Now click on the Restart message at the bottom to restart the Editor.

Follow the rest of tutorial to export from Twinmotion and Import using Datasmith


Changes made to make original 5.1 work with 5.2
===============================================

Edit with Notepad file TwinmotionToUnrealContent.uplugin 

Change the line 
	"EngineVersion": "5.1.0",

to 
	"EngineVersion": "5.2.0",

for UE 5.3 (ue5-main) when launched

Change the line 
	"EngineVersion": "5.1.0",

to 
	"EngineVersion": "5.3.0",


LEGAL STUFF
============
The software and copyright and Assests remains with Epic Unreal Engine and trademarks are protected and respected

The Twinmotion Sofware is described as beta and therefore the is NO WARRANTY AND YOU ARE RESPONSIBLE FOR ANY USAGE OR LOSSES INCURRED

This is NOT A PROFESSIONAL USAGE PATCH AND IS FOR EVALUATION PUPOSES OF UNREAL ENGINE 5.2 AND Twinmotion 2023.1 until such time as official version is launched

