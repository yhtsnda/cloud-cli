# Melanite #
利用SSH协议，远程执行命令的命令行工具。
远程服务器不用安装任何程序，只要开通SSH服务即可。
简单，轻量，配置灵活。

# Feature #

## 远程执行命令 ##
同时发送命令到多台机器执行，获取执行结果并显示。

## 主机分组 ##
可以给主机分组，按照组名执行命令。
一个组可以包含一个或多个主机，一个主机也可以属于一个多个组。

## YAML 描述主机组和主机关系 ##

``` yaml
---
HostGroups:
    - GroupName: groupxxx
      Hosts:
          - Name: xxx
            IP: xxx
            User: xxx
            Password: xxx
            KeyPath: xxx
          - Name: yyy
            IP: yyy
            User: yyy
            Password: yyy
            KeyPath: yyy

    - GroupName: groupyyy
      Hosts:
          - Name: xxx
            IP: xxx
            User: xxx
            Password: xxx
            KeyPath: xxx
          - Name: zzz
            IP: zzz
            User: zzz
            Password: zzz
            KeyPath: zzz
```

# License #
MIT License 2016 (Iota Labs)
