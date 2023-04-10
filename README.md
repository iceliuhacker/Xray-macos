# Xray-macos
```
Mac OS下一键使用的Xray脚本
目前仅支持：
VLESS-XTLS-uTLS-REALITY
VLESS-XTLS-uTLS-Vision
有时间会慢慢增加对接方式。
```
# 使用方法：
## 初次使用：
```
先去该URL：https://github.com/xjasonlyu/tun2socks/releases
下载对应的tun2socks放到当前目录，然后执行：
./xrayctl update	#将自动下载xray以及所需的IP地址库等文件。
```
## 开始使用：
```
./xrayctl
./xrayctl {start|stop|restart|auto|config|subscribe|update} [proxy|tun]
start	#启动
stop	#停止
restart	#重启
auto	#自动选择最快节点【当你有多个节点的时候】
config	#创建新的节点信息
subscribe https://xxxxxxxx/订阅URL	#订阅基于vless的节点
update	#升级xray以及IP库【建议每周执行一次】
可选参数:
proxy	#工作在proxy模式，会自动给系统设置上proxy，然后浏览器等支持系统代理的应用将通过设置的代理上网。
tun	#工作在tun模式，会将用户的【不含系统自身】所有请求转发到xray。【必须有tun2socks才能工作】
```
