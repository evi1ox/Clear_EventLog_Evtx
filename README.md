# clearevtx

声明: 工具仅供安全研究或授权渗透，非法用途后果自负。
PS : 不定期更新
```
C:\Users\Administrator\Desktop>clearevtx-ip.exe Security.evtx 172.16.7.1
[+]PID:2472
Windows Event Log 服务正在启动 .
Windows Event Log 服务已经启动成功。

[+]All Done
```

```
C:\Users\Administrator\Desktop>clearevtx-id.exe Security.evtx 4648
[+]PID:1340
Windows Event Log 服务正在启动 .
Windows Event Log 服务已经启动成功。

[+]All Done
```

```
C:\Users\Administrator\Desktop>logquery.exe
-------------------------------------
LogonTime:      2020/6/12 16:55:19
IpAddress:      10.25.200.44
LogonName:      Administrator
LogonDomain:    WORKGROUP
LogonType:      Logon (RDP)
-------------------------------------
-------------------------------------
LogonTime:      2020/6/11 17:26:24
IpAddress:      10.25.200.73
LogonName:      Administrator
LogonDomain:    WORKGROUP
LogonType:      Logon (RDP)
-------------------------------------
```

Refer:

https://github.com/3gstudent/Eventlogedit-evtx--Evolution
