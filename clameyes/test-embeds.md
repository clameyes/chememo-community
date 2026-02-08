---
title: 機能テスト - URL埋め込み
description: YouTube・Xの自動埋め込みテスト
pubDate: 2026-02-04
tags: [テスト]
author: clameyes
draft: true
---

## YouTube埋め込みテスト

以下のURLが自動的にYouTubeプレイヤーに変換されます（独立した段落のURL）:

https://www.youtube.com/watch?v=dQw4w9WgXcQ

上記のように動画が埋め込まれているはずです。

## X (Twitter) 埋め込みテスト

以下のURLが自動的にXポストに変換されます:

https://twitter.com/astrodotbuild/status/1512144306898976768

ポストが表示されていることを確認してください。

## 通常のリンクテスト

インラインのURL（https://astro.build）は通常のリンクのまま表示されます。

段落内にURLを含む場合も通常のリンクです: https://github.com/withastro/astro はそのままリンクになります。

## リンクカードテスト

以下のURLが自動的にリンクカードに変換されます:

https://github.com/withastro/astro

https://astro.build

https://zenn.dev

上記のように、OGP情報を取得してカード表示されているはずです。

## 通常のリンクカードテスト

https://docs.astro.build/ja/getting-started/

## 注意事項

- **独立した段落**（前後に空行がある）のURLのみが自動変換されます
- インラインのURLや段落内のURLは通常のリンクとして表示されます
- oEmbed対応サービス（YouTube、X、Spotify等）は埋め込み表示になります
- その他の一般的なURLはリンクカード表示になります
