# Block Win Hooks

**BlockWinHooks feature is deprecated.**

_BlockWinHooks_ is a sandbox setting in [Sandboxie Ini](SandboxieIni.md). It specifies whether Sandboxie will allow sandboxed programs to install system-global hooks.

Usage:

```
   .
   .
   .
   [DefaultBox]
   BlockWinHooks=n
```

One application may attach to other applications in the system by employing a mechanism called windows hooks. This mechanism associates a component of the requesting application (called a DLL file) with all other applications.

By default, Sandboxie denies a request to install a global hook, and will instead convert the hook into an application-specific hook, and install this converted hook only into applications running in the same sandbox as the requesting application.

In effect, this restricts the effect of global hooks to a specific sandbox, and increases the protection provided by Sandboxie while still allowing applications that rely on global hooks to execute correctly.

Specifying _BlockWinHooks=n_ disables this protection, and allows a sandboxed application to install global hooks into all running applications, both inside and outside the sandbox.

Related [Sandboxie Control](SP_SBControl.md) setting: [Sandbox Options > Restrictions > Low-Level Access](RestrictionsSettings.md#low-level-access--removed)
