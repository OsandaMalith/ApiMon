# ApiMon
This is a simple Windbg script to monitor common Win32 API calls and display the strings, IPs, Ports, Registry keys passed to the APIs. The Win32 API is huge and I have used common APIs used by programs and malware. I coded this for fun :)

```
Usage: ApiMon.wds run; g;
```

This is a sample output that uses CreateProcess API.

<img src="https://osandamalith.files.wordpress.com/2017/04/1.png">

This is from running netcat. 

<img src="https://osandamalith.files.wordpress.com/2017/04/nc1.png">

<img src="https://osandamalith.files.wordpress.com/2017/04/nc2.png">
