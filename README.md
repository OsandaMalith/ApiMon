# ApiMon
This is a simple Windbg script to monitor common Win32 API calls and display the strings, IPs, Ports, Registry keys passed to the APIs. The Win32 API is huge and I have used common APIs used by programs and malware. I coded this for fun :)

```
Usage: ApiMon.wds run; g;
```

You can remove APIs as you wish to minimize the output or you can add any API you desire. For example
```
bp DLLName!APIName @"$$>a<${$arg0} APIName FileNamePtr

bp kernelbase!CreateFileA @"$$>a<${$arg0} CreateFileA 1";
```

This is a sample output that uses CreateProcess API.

<img src="https://osandamalith.files.wordpress.com/2017/04/1.png">

This is from running netcat. 

<img src="https://osandamalith.files.wordpress.com/2017/04/nc1.png">

<img src="https://osandamalith.files.wordpress.com/2017/04/nc2.png">
