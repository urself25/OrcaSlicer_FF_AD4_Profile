# OrcaSlicer_FF_AD4_Profile
## **Orcalslicer profile for the Flashforge Adventurer 4**

This project will allow a user to add a profile for the Flashforge Adventurer 4 in the official version of Orcaslicer and forks that uses the same structure.

### <ins>**Why use Orcaslicer compared to FlashPrint?**</ins>
While FlashPrint is a fine slicer and perfectly integrated to the Flashforge ecosystem, it does not have the most recent slicing possibility, such as different infill geometries, are not part of it. Orcaslicer provide the flexibility and additional adjustments when slicing models. 

This was based of Orcaslicer V.2.2.0 for Windows. It may be possible to install the same files in MacOS or Linux versions of Orcaslicer but I don't have those OS and can't certify that it is possible.

### <ins>**How to install:**</ins>
Recommendation only: rename file \program files\orcaslicer\resources\profiles\Flashforge.json to Flashforge.json.bk 
Extract the RAR file in \program files\orcaslicer\resources\profiles\ (requires admin rights)
Start OrcaSlicer
Select Adventurer 4 printer

It will overwrite certain common files used among certain Flashforge printers profiles but it should not affect the ability to use them.

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

### <ins>**Versions**</ins>
0.1 - First Release
Changes:
  - Add Flashforge Adventurer 4 profile to Orcaslicer

Known Issues
  - Filament Presets still need work.
    - Flow Rates needs to be adjusted manually
  - LAN/Wifi sliced files transmission from Orcaslicer is not possible and it is unknown if it will ever be.

**Please report any issues or requests 
