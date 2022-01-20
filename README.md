# ChromeRivals Sound Fixes &amp; Enhancements

**This will fix:**
* interrupting standard weapon effect sounds

**This will enhance:**
* overall sound
* 3D sound/surround perception

**[small preview on YouTube](https://youtu.be/BAoE2TniC4o)**

## !! WARNING !!
This guide has been originally uploaded by [jgrnrt](https://github.com/jgrnrt) and re-uploaded by me for the sake of community sharing.
This does not mean that this content is endorsed OR suggested by the ChromeRivals Staff Team, hereby use it at your own risk!

## Installation
(Skip step 1 and 2 if you are not on Windows 10)

1. Install EAX4Unified_redist_4001 & Creative Alchemy 1.45.03
2. Move the CreativeALchemy14503RestrictionRemover-MST.exe to your installed Creative ALChemy directory (C:\Program Files (x86)\Creative\ALchemy), run it as administrator and click "patch".
3. Drag and drop dsound.dll, dsound_aldrv.dll and alsoft.ini into your ChromeRivals directory

## FAQ/Notes
* I installed this mod but I don't get any sound in-game!
Make sure your speaker settings match what's set in alsoft.ini. If you want to use 48000Hz sound output, change it to "frequency=48000Hz" and "default-hrtf=Built-In 48000hz" in alsoft.ini. (44100 & 48000 works both for me)

* The EAX reverb is too loud!
Unfortunately, DSOAL has a bug where it doubles or sometimes quadruples reverb sends when HRTF is active at the same time. The only fix is to adjust the boost= parameter until it sounds right. boost=-6 corresponds to half volume and boost=-12 is quarter volume.

* I'm getting muffled sound in-game!
This seems to be caused by Windows 8 and 10's audio stack. Go into your speaker properies and tick Disable all sound effects under Enhancements. Then, untick "All applications to take exclusive control" under Advanced.
https://answers.microsoft.com/en-us/windows/forum/windows_10-other_settings-winpc/sound-is-muffled-is-there-a-fix/f8b5cf9c-3347-4036-b1a5-7dff5b1da487

* more config tweaks for alsoft.ini: 
https://github.com/kcat/openal-soft/blob/master/alsoftrc.sample



## Original Links:
* https://steamcommunity.com/sharedfiles/filedetails/?id=1384096547
* EAX unified, ALChemy:
https://mega.nz/#!1OwF0QiB!QCXlgNZ5fzppQyqDse-wfjEXsWeRqzNCZlfktgH2-44
(This file may cause false positives with some antivirus programs. Don't be alarmed, it is safe. A statement from the file's creator here:
http://forums.thedarkmod.com/index.php?/topic/18249-tutorial-how-to-setup-eax-for-tdm-on-any-soundcard/&tab=comments#comment-392915
* The restriction remover is neccessary to register your dsound.dll, so DSOAL works properly.
FONVHRTF.3.zip (DSOAL):
https://www.moddb.com/addons/true-3d-sound-for-headphones-hrtf-mod-v131a	
