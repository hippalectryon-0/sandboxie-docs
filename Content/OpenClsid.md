# Open Clsid

_OpenClsid_ is a sandbox setting in [Sandboxie Ini](SandboxieIni.md). It specifies the COM class identifiers for unsandboxed COM objects that should be accessible by a sandboxed program.

Examples:
```
   .
   .
   .
   [DefaultBox]
   OpenClsid={D713F357-7920-4B91-9EB6-49054709EC7A}
```

This example makes the HP Universal Printer Status Monitor pop-up component accessible to sandboxed programs.

Related [Sandboxie Control](SP_SBControl.md) setting: [Sandbox Options > Resource Access > COM Access](ResourceAccessSettings.md#com-access)
