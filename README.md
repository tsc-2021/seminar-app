# セミナーテーマ提案アプリ — セットアップ手順

## 必要なもの
- Cursor（無料） → https://cursor.com
- Google AIのAPIキー（無料） → https://aistudio.google.com
- Vercelアカウント（無料） → https://vercel.com

---

## ステップ1：Gemini APIキーを無料で取得する

1. https://aistudio.google.com にアクセス
2. Googleアカウントでログイン
3. 左メニューの「Get API key」をクリック
4. 「Create API key」ボタンをクリック
5. `AIza...` から始まる文字列をコピーして保存

> クレジットカード不要・完全無料

---

## ステップ2：index.html にAPIキーを設定する

`index.html` を開いて、以下の行を見つけてください：

```
const GEMINI_API_KEY = 'YOUR_API_KEY_HERE';
```

`YOUR_API_KEY_HERE` の部分を、取得したAPIキーに書き換えます：

```
const GEMINI_API_KEY = 'AIzaxxxxxxxxxxxxxxxxxx';
```

---

## ステップ3：Vercelで公開する

1. https://vercel.com にアクセスしてGitHubアカウントでログイン
2. 「Add New Project」→ 画面下部の「Or deploy without a Git repository」→「Upload」を選択
3. このフォルダ（index.html が入っているフォルダ）をドラッグ＆ドロップ
4. 「Deploy」ボタンをクリック
5. 数秒で `https://xxxxx.vercel.app` のURLが発行される

---

## ステップ4：URLを共有する

発行されたURLをLINEやメールで共有するだけです。
相手はアカウント登録不要でアクセスできます。

---

## 注意事項

- APIキーをGitHubなどに公開しないよう注意してください
- Gemini無料枠：1日1,500リクエストまで（通常の使い方では十分です）
- 不明点はClaudeに相談してください
