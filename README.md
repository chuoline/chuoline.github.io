# GitHub Pages 名刺ページ

中小企業の経理フロー改善・AI活用支援用の、静的HTML名刺ページです。

## 公開情報

- **公開URL**: https://chuoline.github.io/
- **公開日**: 2026-06-07
- **リポジトリ**: https://github.com/chuoline/chuoline.github.io

## ファイル構成

- `index.html`
- `style.css`

## 更新手順

内容を変更した場合は以下を実行：

```bash
cd ~/agent-system/github-pages
git add index.html style.css
git commit -m "内容更新"
git push
```

数分で https://chuoline.github.io/ に反映される。

## GitHub Pages 公開手順（初回）

1. GitHubで `chuoline.github.io` リポジトリを作成（Public）
2. `index.html` と `style.css` をpush
3. Settings → Pages → Source: Deploy from a branch / main / root
4. `https://chuoline.github.io/` にアクセスして確認

## 次のアクション

- [ ] QRコード作成（https://qr.io/ などで生成・PNG保存）
- [ ] 名刺データにQRコードを貼り付けて印刷
- [ ] Stripe決済リンク作成後、申込フォームURLを決済リンクに差し替えを検討
- [ ] フェーズ2移行時にHTML LPへのリンクを追加
