# Delete Sandbox Content

[Sandboxie Control](SP_SBControl.md) > [Sandbox Menu](SP_SBControl_SbMenu.md) > Delete Content  
[Sandboxie Control](SP_SBControl.md) > [Tray Icon Menu](SP_TrayIconMenu.md) > Delete Content

![](../Media/SP_DeleteSandboxContent.png)

The _Delete Sandbox_ window appears when the sandbox is about to be deleted. The window is split into two areas:

*   The upper part (about 3/4 of the window) shows the [Recovery](SP_Recovery.md) display and controls, and operates in the same way as the _Quick Recovery_ window. See [Recovery](SP_Recovery.md) for more information.

*   The lower part counts the size of the sandbox (in files, folders, and bytes of disk space) and contains the _Delete Sandbox_ button which initiates delete processing for the sandbox.

The window is displayed when the [Sandbox Menu > Sandbox > Delete Content](SP_SBControl_SbMenu.md#sandbox-menu) command (or the corresponding command from the [Tray Icon Menu](SP_TrayIconMenu.md)) is invoked.

The window is also displayed if the sandbox is configured for automatic delete (see [Sandbox Options > Delete > Invocation](DeleteSettings.md#invocation)), and any files are eligible for [Recovery](SP_Recovery.md). Note that if no files are eligible, the sandbox is deleted silently, without displaying the _Delete Sandbox_ window.

Note that the _Delete Sandbox_ command terminates any programs that are running in the sandbox and initiates the delete process. An empty sandbox will be immediately available to run programs as soon as you click the _Delete Sandbox_ button. While the delete process is undergoing on the old sandbox, the Sandboxie tray icon changes to a red X icon to indicate that sandbox delete is in progress. In correct operation, the red X icon should not remain displayed for more than a few seconds.

* * *

Go to [Recovery](SP_Recovery.md), [Sandboxie Control](SP_SBControl.md), [Help Topics](HelpTopics.md).
