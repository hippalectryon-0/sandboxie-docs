# Enabled

_Enabled_ is a sandbox setting in [Sandboxie Ini](SandboxieIni.md). It is typically specified as _Enabled=y_ (see [Yes Or No Settings](YesOrNoSettings.md)), and indicates that programs can be launched in that sandbox. For example:

```
   .
   .
   .
   [InstallBox]
   Enabled=y
   Enabled=y,Administrators
```

The first example is the typical form of _Enabled_, a required part of any sandbox section in the configuration file. It indicates that the sandbox _InstallBox_ can be used for sandboxing.

The second example similarly defines the sandbox _InstallBox_ while also restricting its use to the Administrators user accounts group. Any user account or group that is recognized by the local Windows system can be specified. Multiple _Enabled_ lines may be specified if the list of user accounts does not fit in one line.

A sandbox that has been restricted to specific users is considered _hidden_ to all other user accounts. Those other user accounts will not see the sandbox listed in [Sandboxie Control](SP_SBControl.md), and any [Forced Processes](SP_ForcedFolderProcess.md#forced-processes) or [Forced Folders](SP_ForcedFolderProcess.md#forced-folders) settings will not apply to those user accounts.

Attempts to explicitly start a program in a sandbox that does not have an associated _Enabled=y_ setting will fail.

Related [Sandboxie Control](SP_SBControl.md) setting: [Sandbox Options > User Accounts](UserAccountsSettings.md)

Related [Sandboxie Control](SP_SBControl.md) command: [Sandbox Menu > Reveal Hidden Sandbox](SP_SBControl_SbMenu.md#reveal-hidden-sandbox)
