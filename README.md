# links — 名刺・二次元コードからのご案内ページ

## 概要
名刺などの印刷物に載せた二次元コードの飛び先となる「中間ページ」。公式チャネル（YouTube／公式LINE／公式X／会社HP）と店舗情報へのリンクを1画面にまとめる。リンク先は `links.json` を編集するだけで差し替えられるため、印刷物の刷り直しが不要。

## 技術スタック
- 静的HTML + JavaScript（フレームワーク・バックエンドなし）
- GitHub Pages

## 公開URL
https://wiseinc-pharmacy.github.io/links/

店舗別表示: `?s=<店舗キー>` を付ける（例: `https://wiseinc-pharmacy.github.io/links/?s=kashiwa`）。
店舗キーは `links.json` の `stores` に定義されたものだけが有効。未定義・無指定の場合は共通リンクのみのトップ表示になる。

## ファイル構成
- `index.html` — ページ本体（`links.json` を読み込んで描画）
- `links.json` — リンク定義（公式チャネルURL・店舗名/住所）。**更新はこのファイルのみ**
- `README.md` — このファイル

## 更新方法
1. `links.json` の該当URL・店舗情報を書き換える（`TBD_` で始まる値は「準備中」扱い）
2. main ブランチへ push すると GitHub Pages に自動反映される

## 更新履歴
- 2026-09-02 初版公開（公式チャネル4リンク＋店舗6件）
