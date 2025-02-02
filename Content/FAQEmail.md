# FAQ Email

Questions and anwers regarding the use of Sandboxie with email software. For a longer discussion, see [Email Protection](EmailProtection.md).

### Q. Why should I use Sandboxie to run my email software?

A. Email software, as any other Internet-facing application, processes data that cannot be completely trusted, as it was received from the Internet. That data -- which is your email -- might contain viruses, and small bits of software designed to exploit vulnerabilities in your email software. By running your email software under the supervision of Sandboxie, you can confine the email software to its sandbox, along with any potential viruses and exploits. See [Email Protection](EmailProtection.md) for more informaion.

### Q. Will Sandboxie identify and delete viruses in my email?

A. No. Sandboxie leaves this task to your anti-virus and anti-malware software. The job of Sandboxie is to provide the first line of defense and prevent a virus from compromising your computer, and potentially even your anti-virus software.

### Q. Message SBIE2212 appears when I run my email software under Sandboxie, does this indicate an error?

A. No. As a safety measure, Sandboxie refuses to run your email program under its supervision, before it has been properly configured. For more information, see the reference page for message [SBIE2212](SBIE2212.md). To learn how to configure support for your email software, see the next question in this FA

### Q. How do I configure Sandboxie for use with my email software?

A. Open [Sandbox Options > Applications > Email Reader](ApplicationsSettings.md#email-reader) and select the email program that you use. If your mailbox data files are not in the default location, see [Sandbox Options > Applications > Folders](ApplicationsSettings.md#folders). Then, you should also test the configuration; see [Test Email Configuration](TestEmailConfiguration.md).

### Q. How do I run my email software under Sandboxie?

A. You can use the _Run Email Reader_ command from the [Sandbox Menu](SP_SBControl_SbMenu.md) or [Tray Icon Menu](SP_TrayIconMenu.md) of [Sandboxie Control](SP_SBControl.md). You can also right-click _Run Sandboxed_ on the program icon for your email software.

### Q. How can I force my email software to always run under Sandboxie?

A. When the program is already running under Sandboxie, go to [Program Settings](ProgramSettings.md#page-1), Page 1, and select the checkbox to _Force program to run in this sandbox_. You can also use [Sandbox Options > Program Start > Forced Programs](ProgramStartSettings.md#forced-programs) to accomplish the same.

### Q. My email software is occasionally updated (automatically or manually). Will the updates take permanent effect?

A. No. The updates will be installed in the sandbox and will disappear when the sandbox is [deleted](DeleteSandboxContent.md). To properly update your email software, run it outside the supervision of Sandboxie, then initiate the update process. If your email software is already set as a forced program (see previous question), use the [Disable Forced Programs](FileMenu.md#disable-forced-programs) command before starting your email software.

### Q. Should I create a separate, dedicated sandbox just for email, or can I use the same sandbox for email and web browsing?

A. This depends primarily on your habits. If you want the convenience of opening your email software by clicking an email ("mailto") link in your browser, then you have to use (and configure) the same sandbox for both web browsing and email reading. On the other hand, some people prefer to isolate the two unrelated types of activities into separate sandboxes. There is no strict answer, and both approaches work well.

### Q. I want to run my web browser in a sandbox, but not my email software. When I click an email link (_mailto_), the web browser starts my email software in the sandbox. What should I do?

A. You can avoid this problem by right-clicking the email link instead of left (normal) clicking it. The right-click menu will let you **copy** the email address. Then switch to your email software and **paste** the email address. If the pasted email address begins with a **mailto:** prefix, then make sure to **delete** that prefix, including the colon (:).

### Q. I want to run my email program in a different sandbox than my web browser. When I click an email link (_mailto_), the web browser tries to start my email software in the wrong sandbox. What should I do?

A. See answer to previous question.

### Q. I have a web mail account and read my email via a web browser, do I need to configure anything?

A. No, because in this case, none of your email is stored in your computer.
