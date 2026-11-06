# altstore-source

mikuta0407 のアプリを配布する [AltStore PAL](https://altstore.io) のソースです。

AltStore で次の URL をソースとして追加してください。

```
https://mikuta0407.github.io/altstore-source/source.json
```

## アプリ

- [mRemote](https://github.com/mikuta0407/mRemote) — iPhone・iPad から RDP と SSH でつなぐアプリ
- [SubDeck](https://github.com/mikuta0407/SubDeck) — Subsonic・Navidrome サーバーで音楽を聴くアプリ

## 構成

- `source.json`: ソース本体。GitHub Pages から配信します
- `apps/<app>/`: アイコンとスクリーンショット
- Releases: Apple が公証した ADP。タグ `<app>-<version>-<build>` ごとに `manifest.json`・`signature`・各 variant の ipa を置き、`source.json` の `assetURLs` から参照します
