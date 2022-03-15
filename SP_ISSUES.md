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
  bit confusing. So far I kept "Sandboxie Control" as the name of the main GUI in the doc.
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
* Used _SettingsGeneralOptions.md#fileOptions_ in _GettingStartedPartFive.md_, but doesn't exist yet (to replace _
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