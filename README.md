# 蓮ノ空 楽曲回収チェッカー

莲之空女学院学园偶像俱乐部（LoveLive! 莲之空）LIVE乐曲回收检查器 — 记录你在演唱会上听过的歌曲！

灵感来源：[水濑祈乐曲回收检查器](https://inori-minase-music-checker.vercel.app/)

在线访问：**https://fhlm.github.io/hasunosora-live-music-checker/**

## 功能

- ✅ 按 LIVE 场次勾选（支持 Day.1/Day.2、昼公演/夜公演 分开选择）
- 📊 自动统计歌曲出现频次排行榜
- 🔍 搜索歌曲名
- 📱 手机端适配（响应式设计）
- 💾 数据本地保存（localStorage）
- 📷 生成图片保存（长按保存）
- 🌐 中日双语切换
- 👤 支持输入用户 ID 个性化图片标题

## 收录数据

数据来源：[LL-Fans](https://ll-fans.jp/data/event)（主要）、萌娘百科、LLWiki

| 年份 | LIVE | 场次 | 曲次 |
|------|------|------|------|
| 2023 | OPENING LIVE EVENT ～Bloom the Dream～ | 2 | 32 |
| 2023 | 1st Live Tour ～RUN！CAN！FUN！～ | 6 | 173 |
| 2024 | 2nd Live Tour ～Blooming with ○○○～ | 4 | 119 |
| 2024 | 103期 Fes×ReC:LIVE ～first crossing～ | 4 | 60 |
| 2024 | みらくらぱーく！ラジオ公開録音 | 3 | 12 |
| 2024 | 3rd Live Tour TRY TRI UNITY!!! | 8 | 132 |
| 2024 | Live & Fan Meeting TRY TRY UNITY!!! | 2 | 28 |
| 2025 | 103期 Fes×ReC:LIVE 追加公演 | 4 | 60 |
| 2025 | 4th Live Dream ～Bloom, The Dream Believers～ | 6 | 178 |
| 2025 | 5th Live Tour ～4Pair Power Spread!!!!～ | 8 | 250 |
| 2026 | 103-105th Fes×ReC:LIVE ～Road to Bloom～ | 4 | 64 |
| 2026 | 6th Live Dream ～Bloom Garden Party～ | 8 | 258 |

**总计：12 个 LIVE · 59 个场次 · 1366 曲次 · 152 独立曲目**

## 部署方法

### GitHub Pages（推荐·免费）

1. Fork 或使用本仓库
2. 进入仓库 **Settings** → **Pages**
3. **Source** 选择 `main` 分支
4. 点击 **Save**
5. 等待 1-2 分钟，访问 `https://你的用户名.github.io/hasunosora-live-music-checker/`

### 本地预览

```bash
# Python
python -m http.server 8080

# 或 Node.js
npx serve .
```

浏览器打开 `http://localhost:8080`

## 数据更新

如需更新曲目数据，可使用爬虫脚本从 LL-Fans 获取：

```bash
# 安装依赖
pip install playwright
playwright install chromium

# 运行爬虫（需启动 Clash 代理，配置在 E:\Tool\VPN配置文件.yaml）
python scrape_hasunosora.py
```

## 联系作者

- QQ: 908283643
- X: [@FeiHuanLuanMan](https://x.com/FeiHuanLuanMan)

## 免责声明

本页面由 AI 自动生成，数据来源于 LL-Fans 等公开网站。虽然已尽力确保准确性，但可能存在错误或遗漏。

本页面仅供个人学习参考使用，不得用于商业用途。如有侵权请联系删除。

## 许可证

本项目为非官方粉丝工具。蓮ノ空女学院スクールアイドルクラブ及 LoveLive! 系列版权归各权利方所有。

数据来源：[LL-Fans](https://ll-fans.jp/data/event)、萌娘百科、LLWiki
