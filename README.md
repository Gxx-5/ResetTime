# ResetTime
用于Linux系统切换到Windows时自动修正系统时间
## ntplib同步时间
从国家授时中心准确时间，调用dos命令修改时间。
授时中心的网址是 cn.pool.ntp.org(注意，流传甚广的210.72.145.44这个ip已经失效了，直接用域名。)
不过从授时中心获取的时间需要ntp协议解析，ntplib就是干这事的。
在dos修改日期时间要通过2个命令实现，date命令修改日期，time命令修改时间。
## pyinstaller打包程序
```bash
pip install pyinstaller
pyinstaller -F -w watermark.py
```
## 添加到Windows开机启动
