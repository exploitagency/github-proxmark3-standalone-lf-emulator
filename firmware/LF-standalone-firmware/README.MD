<pre>
This is the "modded" firmware with standalone LF emulation and standalone cloning enabled.
Dated: 10-7-2018
Commit: ac8a2fded168f1045abf1b227ce2db544479c58f

This is what you want to flash if you don't have standalone LF emulation.

This is the most up to date firmware available as of the time of this posting.
The only mod is removal of HF standalone emulation mode from the makefile thus enabling LF mode.

Also if you want to compile the firmware yourself with LF standalone emulation mode enabled:
Follow general compiling instructions listed in ../../COMPILING-INSTRUCTIONS-KALI-2016.MD plus modify the makefile

On older versions of the proxmark software you will need to modify /armsrc/Makefile
On line 13 remove "-DWITH_ISO14443a_StandAlone"

On newer versions of the proxmark software you will need to modify /common/Makefile_Enabled_Options.common 
On line 6 change "-DWITH_ISO14443a_StandAlone" to "-DWITH_LF_StandAlone"

Instructions for using LF standalone emulation/cloning mode on the elechouse RDV2 and standard version of the proxmark3 can be found at:
https://legacysecuritygroup.com/index.php/categories/9-rfid/7-proxmark-3-emulating-hid-tags-in-standalone-mode
</pre>
