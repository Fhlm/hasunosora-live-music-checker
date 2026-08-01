# 蓮ノ空 楽曲回収チェッカー

蓮ノ空女学院スクールアイドルクラブ（LoveLive! 蓮ノ空）のライブで聴いた楽曲をチェック・管理するためのWebアプリです。

水瀬いのり楽曲回収チェッカー（https://inori-minase-music-checker.vercel.app/）にインスパイアされた非公式ファンツールです。

## 機能

- ✅ LIVEごとに曲目をチェック（localStorageに保存）
- 📊 LIVEごと・全体の回収率表示
- 🔍 曲名・LIVE名で検索
- 📱 スマホ対応レスポンシブデザイン
- 🌸 蓮ノ空テーマカラー

## データについて

データの主要ソースは [LL-Fans](https://ll-fans.jp/data/event) です。萌娘百科、LLWikiも補完データとして使用しています。

現在、以下のLIVEのデータを収録しています：

| 年 | LIVE | データ状態 |
|----|------|-----------|
| 2023 | OPENING LIVE EVENT ～Bloom the Dream～ | ✅ 完全（ll-fans.jp） |
| 2023 | 1st Live Tour ～RUN！CAN！FUN！～ | ✅ 完全（萌娘百科） |
| 2024 | 2nd Live Tour ～Blooming with ○○○～ | ✅ 完全（萌娘百科） |
| 2024 | 103期 Fes×ReC:LIVE ～first crossing～ | ✅ 完全（萌娘百科） |
| 2025 | 103期 Fes×ReC:LIVE 追加公演 | ⚠️ 未収録 |
| 2025 | 3rd Live Tour TRY TRI UNITY!!! | ⚠️ 神奈川公演のみ |
| 2025 | 4th Live Dream | ⚠️ 未収録 |
| 2025 | 5th Live Tour ～4Pair Power Spread!!!!～ | ⚠️ 東京Day1のみ |
| 2026 | 103-105th Fes×ReC:LIVE ～Road to Bloom～ | ⚠️ 未収録 |
| 2026 | 6th Live Dream ～Bloom Garden Party～ | ⚠️ 未収録 |

> ⚠️ データの追加・修正は大歓迎です！Pull Requestをお待ちしています。
> 
> より詳細なデータは [LL-Fans](https://ll-fans.jp/data/event) で確認できます（MC情報、初披露マーク、衣装情報など）。
> `scrape_hasunosora.py` を使ってLL-Fansからデータを一括取得可能です（要: `pip install playwright && playwright install chromium`）。

## GitHub Pages でデプロイする方法

### 方法1：GitHub Pages（推奨・無料）

1. GitHubで新規リポジトリを作成（例: `hasunosora-music-checker`）
2. このフォルダのファイルをリポジトリにプッシュ：

```bash
cd hasunosora-music-checker
git init
git add .
git commit -m "Initial commit: 蓮ノ空楽曲回収チェッカー"
git remote add origin https://github.com/あなたのユーザー名/hasunosora-music-checker.git
git branch -M main
git push -u origin main
```

3. GitHubのリポジトリページ → **Settings** → **Pages**
4. "Source" を **Deploy from a branch** に設定
5. Branch を `main` / `/(root)` に設定 → **Save**
6. 数分後、`https://あなたのユーザー名.github.io/hasunosora-music-checker/` でアクセス可能に！

### 方法2：Vercel（無料）

1. [Vercel](https://vercel.com) にGitHubアカウントでログイン
2. "New Project" → リポジトリをインポート
3. そのままDeploy（設定不要、index.htmlを自動検出）
4. `https://hasunosora-music-checker.vercel.app` のようなURLが発行される

## ローカルでプレビュー

```bash
# Pythonで簡易サーバー
python -m http.server 8080

# または Node.js で
npx serve .
```

ブラウザで `http://localhost:8080` を開く。

## ライセンス

このプロジェクトはファンメイドの非公式ツールです。蓮ノ空女学院スクールアイドルクラブおよびLoveLive!シリーズの著作権は各権利者に帰属します。

データソース：LL-Fans、萌娘百科、LLWiki、LoveLive!公式
