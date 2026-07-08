Command Injection Section (Wireshark Capture)
----------------------------------------------
Command Injection Attempt (Captured in Wireshark)
-------------------------------------------------
Overview
--------

Tested for Command Injection vulnerabilities in the OWASP Juice Shop application by injecting OS commands into user-controlled fields.
Tools Used

Burp Suite,
Wireshark,
OWASP Juice Shop

Methodology & Steps
--------------------

Identified potential injection points (search bar, complaint form).
Injected common command injection payloads:
; whoami 
& whoami
| whoami
$(whoami)

Monitored both application response and network traffic in Wireshark.

Key Findings

No visible output in the application interface.
Captured the injected payloads in HTTP requests via Wireshark, confirming they were sent to the server.
The server did not return command output, suggesting either proper filtering or blind command injection.

What I Learned
----------------

Command Injection occurs when user input is passed to system commands without proper sanitization.
Even if output is not visible, the payload may still be executed (blind injection).
Wireshark is essential for capturing network-level evidence when the application does not show results.
Proper input validation and use of parameterized commands are critical defenses.

Security Takeaways

Never pass user input directly to system commands.
Use safe APIs or libraries that prevent command execution.
Implement allowlisting for acceptable input.
