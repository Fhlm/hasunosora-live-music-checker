# LIVE 楽曲回収チェッカー

LoveLive! 系列 LIVE 乐曲回收检查器 — 记录你在演唱会上听过的歌曲！

支持系列：🪷 蓮ノ空女学院 / 🌈 虹ヶ咲学園

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
- 🎨 系列主题色切换（莲之空粉色 / 虹咲橙色）

## 收录数据

数据来源：[LL-Fans](https://ll-fans.jp/data/event)（主要）、萌娘百科、LLWiki

### 🪷 蓮ノ空女学院

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

**莲之空总计：12 个 LIVE · 59 个场次 · 1366 曲次**

### 🌈 虹ヶ咲学園

| 年份 | LIVE | 场次 | 曲次 |
|------|------|------|------|
| 2019 | 校内マッチングフェスティバル | 2 | 20 |
| 2019 | First Live "with You" | 2 | 43 |
| 2020 | 2nd Live! Brand New Story / Back to the TOKIMEKI | 2 | 49 |
| 2021 | 校内シャッフルフェスティバル | 2 | 32 |
| 2021 | 3rd Live! School Idol Festival | 2 | 48 |
| 2021-22 | UNIT LIVE & FAN MEETING | 8 | 90 |
| 2022 | 4th Live! ～Love the Life We Live～ | 2 | 50 |
| 2022 | 5th Live! 虹が咲く場所 | 4 | 115 |
| 2023 | UNIT LIVE! | 8 | 176 |
| 2023 | にじたび！TOKIMEKI FAN MEETING TOUR | 18 | 144 |
| 2023-24 | 6th Live! I love You ⇆ You love Me | 4 | 119 |
| 2024 | 7th Live! NEW TOKIMEKI LAND | 2 | 58 |
| 2025 | FMT ニジガク校外学習 | 18 | 144 |
| 2026 | FLOWER MUSIC LIVE | 2 | 44 |
| 2026 | 8th Live! TOKIMEKI Express | 4 | 137 |

**虹咲总计：15 个 LIVE · 64 个场次 · 872+ 曲次**

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

## 联系作者

- QQ: 908283643
- X: [@FeiHuanLuanMan](https://x.com/FeiHuanLuanMan)

## 免责声明

本页面由 AI 自动生成，数据来源于 LL-Fans 等公开网站。虽然已尽力确保准确性，但可能存在错误或遗漏。

本页面仅供个人学习参考使用，不得用于商业用途。如有侵权请联系删除。

## 许可证

本项目为非官方粉丝工具。蓮ノ空女学院スクールアイドルクラブ、虹ヶ咲学園スクールアイドル同好会及 LoveLive! 系列版权归各权利方所有。

数据来源：[LL-Fans](https://ll-fans.jp/data/event)、萌娘百科、LLWiki
