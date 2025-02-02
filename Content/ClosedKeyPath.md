# Closed Key Path

_ClosedKeyPath_ is a sandbox setting in [Sandboxie Ini](SandboxieIni.md). It specifies path patterns for which Sandboxie will deny _all_ access by sandboxed progams, including _read_ access. This setting essentially blocks registry keys from being accessed by sandboxed programs.

[Program Name Prefix](ProgramNamePrefix.md) may be specified.

Example:

```
   .
   .
   .
   [DefaultBox]
   ClosedKeyPath=!msimn.exe,HKEY_CURRENT_USER\Software\Microsoft\Internet Account Manager
```

The example blocks any program _other than_ Outlook Express (_msimn.exe_) from accessing the registry key containing configured email accounts for the active user account.

The value specified for _ClosedKeyPath_ can include wildcards, although for registry keys, the use of wildcards is rarely needed. For more information on this, including examples that show the use of wildcards, see [OpenFilePath](OpenFilePath.md). (_OpenFilePath_ deals with files, not registry keys, but the principle of using wildcards remains the same.)

**Note:** this setting does not apply to _sandboxed_ items. It only blocks access to items outside the sandbox, that have not yet been copied into (or created) in the sandbox.

**Note:** Unlike the corresponding [OpenKeyPath](OpenKeyPath.md) setting, the _ClosedKeyPath_ settings always applies to sandboxed programs, whether the program executable file resides within the sandbox, or out of it.

Related [Sandboxie Control](SP_SBControl.md) setting: [Sandbox Options > Resource Access > Registry Access > Blocked Access](ResourceAccessSettings.md#registry-access--blocked-access)

* * *

Go to [Sandboxie Ini](SandboxieIni.md).
