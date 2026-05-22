# こころBot Landing Page

## デプロイ方法（Netlify）

1. このフォルダをNetlifyにドラッグ＆ドロップ、またはGitHub連携でデプロイ
2. カスタムドメインを設定

## ロゴ差し替え

1. ロゴ画像を `images/` フォルダに配置
2. `index.html` 内の以下を変更：

```html
<!-- 削除 -->
<div class="logo-placeholder">ロゴ</div>

<!-- コメント解除して画像パス指定 -->
<img src="images/logo.png" alt="こころBot" class="logo-img">
```

## CTA リンク設定

`index.html` 内の `href="#"` を実際のLINE友達追加URLに差し替え：

```html
<a href="https://line.me/R/ti/p/YOUR_LINE_ID" class="cta-btn">
```

## ファイル構成

```
kokoro-bot-lp/
├── index.html      ← メインLP
├── netlify.toml     ← Netlify設定（ヘッダー・キャッシュ）
├── images/          ← ロゴ・画像格納先
└── README.md        ← このファイル
```
