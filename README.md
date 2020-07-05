# Clear_EventLog_Evtx

声明: 工具仅供安全研究或授权渗透，非法用途后果自负。

目的: 清除 RDP 记录

### clearevtx-ip.exe  

- 清理IP(172.16.7.1)所有记录

```
C:\Users\Administrator\Desktop>clearevtx-ip.exe Security.evtx 172.16.7.1
[+]PID:2472
Windows Event Log 服务正在启动 .
Windows Event Log 服务已经启动成功。

[+]All Done
```


### clearevtx-id.exe
- 清理事件ID(4648)所有记录
```
C:\Users\Administrator\Desktop>clearevtx-id.exe Security.evtx 4648
[+]PID:1340
Windows Event Log 服务正在启动 .
Windows Event Log 服务已经启动成功。

[+]All Done
```


### logquery.exe

- 查询远程和本地登录的ip和时间
- 攻击者可以用于侦查管理员上线时间以及频繁登录的ip做相关信息收集, 以及避免不必要的尴尬😓
- 运维人员自然是用来找攻击者痕迹

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


PS : 不定期更新

Refer:

[https://github.com/3gstudent/Eventlogedit-evtx--Evolution](https://github.com/3gstudent/Eventlogedit-evtx--Evolution)

[https://github.com/QAX-A-Team/EventLogMaster/tree/master/powershell](https://github.com/QAX-A-Team/EventLogMaster/tree/master/powershell)

