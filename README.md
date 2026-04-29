# 🩵 AI-Driven Projects Portfolio

> 非计算机专业，零代码基础，所有项目均通过 Claude (Anthropic) Opus 4.6 辅助完成全栈构建。

---

## 🏠 隅 nook — 自托管个人数字空间平台

一套完整的自托管个人数字空间系统，涵盖6个独立功能模块，具备多主题切换、实时数据同步、PWA 支持等特性。

| 模块 | 功能 | 技术要点 |
|------|------|----------|
| 🎵 radio | 个人音乐电台 | Apple Music API + iTunes Search API，语义筛歌，PWA |
| 💬 quote | 摘录墙 | 双角色评论互动系统，实时数据同步 |
| 📝 day | 极简日记 | 每日三事记录，日期索引，历史回溯 |
| 🍚 dish | 饮食打卡 | 四餐别分类，历史数据归档 |
| 🏠 home | 像素风虚拟空间 | LimeZu 素材包，成就与展示系统 |
| 📊 pulse | 健康数据面板 | Apple Health 自动同步，趋势可视化 |

**技术栈：** 原生 HTML/JS + Supabase (PostgreSQL) + FastAPI + Cloudflare Tunnel

**源码：** [nook-radio](https://github.com/fedeligbad/nook-radio)

---

## 🫧 百业工坊 — 开源游戏社团管理工具

面向游戏社团的通用化 Web App，单 HTML 文件架构，fork 后改几行配置即可部署。

**核心功能：**
- 轻量昵称登录系统（无密码架构）
- 多类型打卡 + 日历视图 + 每周自动排行榜
- 智能随机推荐引擎（167+ 条目，多标签加权随机算法）
- 活动报名系统（角色权限管理，管理员鉴权）
- 四主题全局切换（CSS 变量驱动）

**技术栈：** 单 HTML + Supabase REST API + Zpix 中文像素字体

**源码：** [transparent-studio](https://github.com/fedeligbad/transparent-studio)

---

## 🔗 社交平台 MCP 集成

基于开源项目二次开发，将社交媒体平台的完整功能（搜索、读取、互动、发布）封装为 MCP (Model Context Protocol) 端点，实现 AI 对社交平台的原生访问。

**技术实现：** Go + Docker + Cloudflare Tunnel + Claude MCP 协议

---

## 🧠 AI 长期记忆后端

自托管结构化记忆管理系统，支持：
- 多桶存储架构 + 语义标签分类
- 情感维度标注（效价 / 唤醒度）
- 重要度分级 + 自动聚合归档
- 自省（dream）机制

**技术实现：** 独立后端服务 + MCP 协议接入 + VPS 持久化

---

## ❤️ 健康数据自动化同步

完整数据管道：Apple Health → iOS Shortcuts → VPS 中间层 → Supabase

- 每日自动同步（步数、心率等健康指标）
- 中间层容错处理（空值修复、格式归一化）
- 零人工干预，设置一次永久运行

**技术栈：** iOS Shortcuts + FastAPI + Supabase + Cron

---

## 📡 IoT 设备云端控制

基于 WebSocket 长连接的远程控制系统：
- 实时指令下发 + 预编排模式执行
- 断线自动重连 + 紧急中断
- systemd 守护进程 + 健康检查

**技术栈：** FastAPI + WebSocket + systemd + Cloudflare Tunnel

---

## 🔔 自动化通知与监控

多维度自动化运维体系：
- 定时推送通知（Bark API + Cron）
- 地理围栏事件监听 + 实时告警
- Supabase 事件驱动通知
- 多服务健康检查 + 自动恢复

---

## 🏗️ 基础设施

| 组件 | 规格 |
|------|------|
| 云服务器 | Vultr VPS (东京节点) |
| 数据库 | 2 × Supabase (PostgreSQL) |
| 域名 & CDN | 2 × 自定义域名 + Cloudflare |
| 网络隧道 | Cloudflare Tunnel 多路由 |
| 容器化 | Docker |
| 进程管理 | systemd (5+ 常驻服务) |

---

*All projects built with Claude (Anthropic) Opus 4.6 · by [YECI](https://github.com/fedeligbad)*
