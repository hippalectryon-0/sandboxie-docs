# Open Credentials

_OpenCredentials_ is a sandbox setting in [Sandboxie Ini](SandboxieIni.md). It is typically specified as _OpenCredentials=yes_ (see [Yes Or No Settings](YesOrNoSettings.md)), and indicates that Sandboxie should not isolate Windows credentials in the sandbox. For example:
```
   .
   .
   .
   [DefaultBox]
   OpenCredentials=yes
```

Indicates that programs running in the DefaultBox sandbox will update the real credential store, rather than a sandboxed instance of it.

Windows credentials are used primarily by Windows and Microsoft applications to store user name and password information for:

*   Network shares
*   Microsoft accounts

To manage Windows credentials, start Control Panel > User Accounts, select an account, and the click on the Related Task labeled _Manage my network passwords._

**Note:** Sandboxie stores credentials in the sandboxed protected storage. Thus, if the setting _Save outside sandbox: History of search strings and invoked commands_ in [Sandbox Options > Applications > Web Browser](ApplicationsSettings.md#web-browser) is enabled, credentials will not be stored in the sandbox, regardless of the OpenCredentials setting.

Related [Sandboxie Control](SP_SBControl.md) setting: _Save outside sandbox: Account information for Hotmail and Messenger_ in [Sandbox Options > Applications > Web Browser](ApplicationsSettings.md#web-browser)
