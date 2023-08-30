# Installation exit codes

The setup program may return one of the following exit codes:

<table><thead><tr><th width="141" align="right">Exit code</th><th>Definition</th></tr></thead><tbody><tr><td align="right">0</td><td>Setup was successfully run to completion or the /HELP or /? command line parameter was used.</td></tr><tr><td align="right">1</td><td>Setup failed to initialize.</td></tr><tr><td align="right">2</td><td>The user clicked Cancel in the wizard before the actual installation started, or chose “No” on the opening “This will install…” message box.</td></tr><tr><td align="right">3</td><td>A fatal error occurred while preparing to move to the next installation phase (for example, from displaying the pre-installation wizard pages to the actual installation process). This should never happen except under the most unusual of circumstances, such as running out of memory or Windows resources.</td></tr><tr><td align="right">4</td><td><p>A fatal error occurred during the actual installation process.</p><p><em>Note:</em> Errors that cause an Abort-Retry-Ignore box to be displayed are not fatal errors. If the user chooses <em>Abort</em> at such a message box, exit code 5 will be returned.</p></td></tr><tr><td align="right">5</td><td>The user clicked Cancel during the actual installation process, or chose <em>Abort</em> at an Abort-Retry-Ignore box.</td></tr><tr><td align="right">6</td><td>The Setup process was forcefully terminated by the debugger (<em>Run | Terminate</em> was used in the Compiler IDE).</td></tr></tbody></table>

Before returning an exit code of 1, 3 or 4 an error message explaining the problem will normally be displayed.

Future versions may return additional exit codes, so applications checking the exit code should be programmed to handle unexpected exit codes gracefully. Any non-zero exit code indicates that Setup was not run to completion.