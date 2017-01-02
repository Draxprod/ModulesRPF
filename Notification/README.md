# ModulesRPF

## License (Custom)
You can edit the script whitout my permission but you are not allow to remove the credit (but you can add "Edit by : Your Name" )
You are not allowed to sell my script!

## Installing
1. Download all files for the module you are installing and **read the module's README.md**
2. Navigate to **RPFramework.yourMap\Functions\modules** and place the module's folder there
3. Navigate to **RPFramework.yourMap\Functions\modules\CONFIG** and open up **moduleDialogs.hpp**, **moduleFunctions.hpp**, **moduleRscTitles.hpp**, **moduleSounds.hpp**
4. In **moduleDialogs.hpp**, **moduleFunctions.hpp**, **moduleRscTitles.hpp** and **moduleSounds.hpp** add a new line in format `#include "..\MODULE\CURRENTFILESUFFIX.hpp"` where **CURRENTFILESUFFIX** is the "suffix" of the current file. For **moduleFunctions.hpp** the **CURRENTFILESUFFIX** would be **Functions**.

## Usage
Function provided: `ClientModules_fnc_showNotification`

Parameter(s):
_title 		: STRING - Default Value  : ""
_text 		: STRING - Default Value  : ""
_stripColor	: ARRAY  - Default Value  : [0.043,0.486,0.769,1]
_sound 		: STRING - Default Value  : "additemfailed"

If you don't want to use sound, add "" in the fourth params. ["Error","Oops it's not possible my friend",nil,"mySound"]
If you want a sound but you don't want to change the strip color, use nil as third params : ["Error","Oops it's not possible my friend",nil,""]

Exemple : ["Error","Oops it's not possible my friend",nil,""] call ClientModules_fnc_showNotification;