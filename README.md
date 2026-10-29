# 逆再生チャレンジ サイト

アプリ「逆再生チャレンジ」の紹介・サポート・プライバシーポリシーの、GitHub Pages 用の静的サイト。

- `index.html`: 紹介（App Store の「マーケティング URL」に使える）
- `support.html`: サポート（App Store の「サポート URL」）
- `privacy.html`: プライバシーポリシー（App Store の「プライバシーポリシー URL」）

## 公開前に直すところ

- 連絡先のメールアドレス: `support.html` の `REPLACE_WITH_EMAIL`（2 か所）
- App Store のボタン: `index.html` の「App Store で公開予定」を、公開後にストアの URL に置き換える

```bash
grep -rn REPLACE_WITH_EMAIL .
```

## 公開（GitHub Pages）

リポジトリの Settings → Pages → Build and deployment で、Branch を `main` / `/ (root)` にする。
URL は `https://<ユーザー名>.github.io/reverse-audio-challenge-site/`。

## 手元で見る

```bash
python3 -m http.server 8000
```
