# Comment

Current workflow: once I've gone through updating a page, I prefix it with _SP__. Some non-prefixed pages may be
modified, this means that they've been modified partially (ex: renaming an image) but I haven't properly updated them
yet.

All the non-SP items will be reverted to their original values once we're done, so as not to disturb the original Legacy
Sandboxie documentation.

# Issues found in updating the doc

* The doc changes related to SB-Plus are precesed bu _SP__ (ex _SP_README.md_). We need to revert all the other (non-SP)
  files to the original branch's values before doing the PR once we're finished.
* The old sandboxie calls the main GUI "Sandboxie Control", but the new one is just called "Sandboxie Plus", which
  conflicts with the name of the program. Therefore the portions of the doc that refer to "Sandboxie Control" may be a
  bit confusing. So far I kept "Sandboxie Control" as the name of the main GUI in the doc. Same issue with "Programs
  View", which is now unnamed.
* Shouldn't _Help>Online Documentation_ redirect here (https://sandboxie-plus.github.io/sandboxie-docs) rather
  than https://sandboxie-plus.com/ ?
* Changed _Quick Recovery_ to _Recovery_ to reflect the SB-Plus UI with a "brutal" replacement, might have missed a few
  places to rewrite
* In GettingStartedPartFour.md, it is said "recoverable folders by default are your _Documents_ folder and the Windows _
  Favorites_ folder. Where applicable, your _Downloads_ folder is also considered a recoverable folder.". In the sandbox
  settings it shows three folders: %Desktop%, %Personal% and %{374DE290-123F-4565-9164-39C4925E467B}%. Is the message in
  GettingStarted still accurate ?
* https://github.com/sandboxie-plus/Sandboxie/issues/1692 > when resolved, reflect the chosen behavior in
  GettingStartedPartFive.md and DeleteSandbox.md
* Used _SBOptions_GeneralOptions.md#fileOptions_ in _GettingStartedPartFive.md_, but doesn't exist yet (to replace _
  DeleteSettings.html#invocation_)
* The doc mentions the Sandboxie Forums in several instances. While https://sandboxie-plus.com/ redirects
  to https://forum.xanasoft.com/, the github issues seem to indicate that the current forum
  is https://www.wilderssecurity.com/forums/sandboxie-sbie-open-source-plus-classic.144/. We need to decide which forum
  we put forward, and reflect that in the doc (many places, do a global search on _Favorites_)
* There's a general confusion in the doc between _deleleting a sandbox_ and _deleting a sandbox's content_, which should
  be clarified
* What does the "Remember target selection" dropdown do when checked ? Whether checked or not, the location does not
  change after recovering an item, and is not selected when opening the recovery window again. _Once clarified > update
  Recovery.md_
* Need to create _SBControl_ViewMenu.md_
* Need to create _SBControl_LogView.md_ for _Sbie Messages_, _Trace Log_
* When creating a new box, if you input bad characters in the name, it says "The sandbox name can contain only letters,
  digits and underscores which are displayed as spaces." However, spaces can also be used. Moreover, it's not clear
  whether there's a difference between underscores and spaces. Upon investigation, it would seem that underscores and
  spaces are treated the same (can't create both "a a" and "a__a" sandbox)
  . (https://github.com/sandboxie-plus/Sandboxie/issues/1693 When resolved, update _SandboxMenu.md_)
* Need to create _BoxTypePresets.md_, or create one .md per type of preset and list them in _SandboxMenu.md_
* SBControl>Sandbox>Create Box Group: What does this do ? Why does the "?" button do nothing ? Why can we create a group
  with the same name twice ? (solved > create BoxGroups.md. Line to consider: "Related [Sandboxie Ini](SandboxieIni.md)
  setting: BoxDisplayOrder.")
* ![](Media/temp_1.png) Why do we have twice [None] ? Why is move up/down always greyed ? Why don't the groups have the
  group icon (in the creation menu) instead of a sandbox icon ?
* "Pause Forcing Programs" > same UI issue as "Create Box Group", the "?" button doesn't do anything. Also: would be
  nice to have an indicator of remaining time.
* SBControl > Sandbox > Maintenance: What do those options do ? (> SandboxMenu.md, or their own .md file))