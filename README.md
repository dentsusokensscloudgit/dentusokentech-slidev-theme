# 電通総研テクノロジー Slidev テーマ

PowerPointテンプレート `v1.0.0` から変換したMarpカスタムテーマです。

## ファイル構成

```
dentusokentech-slidev-theme/
├── layouts/
│   ├── default.vue      # 通常スライド
│   ├── cover.vue        # 表紙
│   ├── section.vue      # セクション区切り
│   ├── confidential.vue # CONFIDENTIALマーク付き
│   └── blank.vue        # 白紙
├── public/
│   ├── logo.png         # ロゴ画像（大）- 表紙用
│   └── logo-small.png   # ロゴ画像（小）- 右上表示用
├── setup/
│   └── shiki.ts         # シンタックスハイライト設定
├── style.css            # テーマスタイル本体
├── slides.md            # サンプルスライド（エントリポイント）
├── package.json         # プロジェクト設定
└── README.md            # このファイル
```

## セットアップ

```bash
npm install
npm run dev
```

## コマンド

| コマンド | 説明 |
|---------|------|
| `npm run dev` | 開発サーバー起動 |
| `npm run build` | 静的サイトビルド |
| `npm run export` | PDFエクスポート |

## レイアウト

Markdownのフロントマターでレイアウトを切り替えます:

| レイアウト | 用途 |
|-----------|------|
| (default) | 通常コンテンツ |
| `cover` | 表紙 |
| `section` | セクション区切り |
| `confidential` | 機密マーク付き |
| `blank` | 白紙 |

### 使用例

```markdown
---
layout: cover
---

# タイトル
```

## テーマカラー

| 名前 | HEX | 用途 |
|------|-----|------|
| Accent1 (Green) | `#39B382` | メインカラー、装飾、箇条書き |
| Accent2 (Red) | `#CE3E04` | 強調テキスト |
| Accent3 (Yellow) | `#F3C500` | - |
| Accent4 (Blue) | `#6FA4CE` | - |
| Accent5 (Purple) | `#8C6BA4` | - |
| Accent6 (Pink) | `#EE488D` | - |
| Dark1 | `#000000` | 本文テキスト |
| Dark2 | `#646464` | サブテキスト、装飾 |
| Link | `#467886` | ハイパーリンク |

## フォント

- メイン: **BIZ UDPゴシック**
- コード: **Consolas** (フォールバック: BIZ UDPゴシック)
