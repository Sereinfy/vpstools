# vpstools

更新
```
apt update -y && apt install -y curl socat wget git sudo
```
时区
```
timedatectl set-timezone Asia/Shanghai

timedatectl
```
# VPS 测试 & 优化脚本合集

整理了一些常用的 VPS 测试、检测和优化脚本，支持一键运行。

---

## 📺 流媒体解锁检测
用于测试 IP 是否支持 Netflix、Disney+、YouTube Premium 等流媒体平台。
```
bash <(curl -Ls unlock.icmp.ing/scripts/test.sh)
```
```
bash <(curl -sL Media.Check.Place)
```
---

## 🌍 IP 质量体检
检测 IP 质量（ASN、地理位置、黑名单、延迟等）。
```
bash <(curl -sL IP.Check.Place)
```
---

## 🔄 三网回程路由测试
测试回程路由，分析服务器到 **电信 / 联通 / 移动** 的回程线路。
```
curl -sSf https://raw.githubusercontent.com/zhanghanyun/backtrace/main/install.sh | sh
```
---

## 📶 网络质量
测试当前网络的延迟、路由、丢包等综合指标。
```
bash <(curl -Ls https://Check.Place) -N
```
---

## 🧰 综合性能测试
包含网络带宽、硬盘性能、CPU 性能等测试工具。

# 常用综合测试脚本
```
wget -qO- bench.sh | bash
```
## Yet-Another-Bench-Script（更详细，支持 Geekbench）
```
curl -sL yabs.sh | bash -s -- -i
```
## 融合怪
```
bash <(wget -qO- ecs.0s.hk)
```
---

## 📦 常用工具与优化项目

- [VPSDance/scripts](https://github.com/VPSDance/scripts)  
  🔹 各类 VPS 测试脚本集合。

- [ylx2016/Linux-NetSpeed](https://github.com/ylx2016/Linux-NetSpeed)  
  🔹 TCP 加速优化，支持 **BBR/锐速** 等。

- [mack-a/v2ray-agent](https://github.com/mack-a/v2ray-agent)  
  🔹 V2Ray/XTLS/Trojan 一键脚本，支持多协议。
- [ike-sh/bbrv3-lite](https://github.com/ike-sh/bbrv3-lite)  
  🔹 轻量级 BBR v3 / XanMod / TCP 网络调优脚本 
- [fscarmen/sing-box](https://github.com/fscarmen/sing-box)  
  🔹 Sing-box 一键脚本，支持多种代理协议和面板。

---


