# OrcaSlicer_FF_AD4_Profile
## **STATUS UPDATE AND FUTURE OF THIS PROJECT**
2025/03/07: The Adventurer 4 profile has been approved for integration into the next iteration of Orcaslicer. This means that installation of seperate files will no longer be needed and the Adventurer 4 profile files will not be updated.

<ins>**Next steps: Adventurer 4 Pro**</ins>
While I don't own an Adventurer 4 Pro, I will do my best to make a profile for Orcaslicer. As such, testers will be needed to try it out and report any issues. A first attempt is already available under the Releases as V0.5. Next releases will however be based on the next iteration of Orcaslicer and previous versions will not be supported. 

## **Orcalslicer profile for the Flashforge Adventurer 4**

This project will allow a user to add a profile for the Flashforge Adventurer 4 in the official version of Orcaslicer and forks that uses the same structure.

**Until release of V1.0, current releases are still experimental and not all values included in the presets may be perfectly adjusted for the Adventurer 4 printer. While it will not brick your printer, print quality may not be optimal.**

### <ins>**Why use Orcaslicer over FlashPrint?**</ins>
While FlashPrint is a fine slicer and perfectly integrated to the Flashforge ecosystem, it does not have the most recent slicing possibility, such as different infill geometries, are not part of it. Orcaslicer provide the flexibility and additional adjustments when slicing models. 

This was based of Orcaslicer V.2.2.0 for Windows. It may be possible to install the same files in MacOS or Linux versions of Orcaslicer but I don't have those OS and can't certify that it is possible.

### <ins>**How to install:**</ins>
_Recommendation only: rename file "\program files\orcaslicer\resources\profiles\Flashforge.json" to "Flashforge.json.bk"_
Certain files will overwrite certain common files used among certain Flashforge printers profiles but it should not affect the ability to use them.

#### Under Windows ####
- Extract the RAR file in \program files\orcaslicer\resources\profiles\ (requires admin rights)
- Start OrcaSlicer
- Select Adventurer 4 printer

#### Under MacOS #### 
Thanks to @lcoppenr for the steps

- Open OrcaSlicer
- Goto Help - Show Configuration Folder
- Leave the Finder windows with the configuration Folder open, but close OrcaSlicer
- In the Finder window for the Configuration Folder, under System, delete Flashforge.json and the Flashforge folder if they exist. They existed for me as I had selected the Adv3 just to see what OrcaSlicer was like. On a clean install they may not exist.
- Download the repository zip file (automatically extracts to Downloads typically)
- Select and Copy the Flashforge.json and the Flashforge folder in the newly extracted download. (don't paste them anywhere yet)
- Open Finder and the Applications folder
- Two finger click or Right click on OrcaSlicer application and select Show Package Contents
- Under Contents/Resources/profiles, Paste the previous copied Flashforge.json and Flashforge folder.
- You'll be asked to Replace or Merge the Folders. You want to Merge them
- Next you will be asked to Keep Both, Stop or Replace Flashforge.json. Select Replace
- Open OrcaSlicer
- You should see the Adventurer 4 in the printer selection list with 0.3, 0.4,0.6 nozzles and generic filaments.

### <ins>**How to remove**</ins>
#### **"Easy" method**
Uninstall OrcaSlicer, then delete the following folders and files 
  "\program files\orcaslicer\resources\profiles\Flashforge"; 
  "\Users\<your username>\AppData\Roaming\OrcaSlicer\system\Flashforge\"; 
  "\Users\<your username>\AppData\Roaming\OrcaSlicer\system\Flashforge.json"
Reinstall Orcaslicer

#### **More complex method**
Delete some extracted files in the following folders
  "\program files\orcaslicer\resources\profiles\Flashforge\"; 
  "\Users\<your username>\AppData\Roaming\OrcaSlicer\system\Flashforge\";
    "\program files\orcaslicer\resources\profiles\Flashforge\machine"; 
    "\Users\<your username>\AppData\Roaming\OrcaSlicer\system\Flashforge\machine";
    "\program files\orcaslicer\resources\profiles\Flashforge\process"; 
    "\Users\<your username>\AppData\Roaming\OrcaSlicer\system\Flashforge\process";
    "\program files\orcaslicer\resources\profiles\Flashforge.json"; 
    "\Users\<your username>\AppData\Roaming\OrcaSlicer\system\Flashforge.json";
  Rename
      "\program files\orcaslicer\resources\profiles\Flashforge.json.bk" to "\program files\orcaslicer\resources\profiles\Flashforge.json"
  * Leaving the overwriten files under the /filament folders should not pose a problem. If it does, a complete reinstall of Orcaslicer using the above Easy Method would be necessary.

#### <ins>**New Orcaslicer versions**</ins>
Until such a time the Adventurer 4 profile is added to Orcaslicer official releases, the profile will need to be reinstall after each software update.

### <ins>**How to use:**</ins>
  - Import your model files in orcaslicer, adjust the needed settings and slice.
  - To send file to printer
    - Save Gcode file to a USB drive and insert the drive to the printer and build; or,
    - Save Gcode on your computer, open Flashprint, load the Gcode file and click on send to printer button.
