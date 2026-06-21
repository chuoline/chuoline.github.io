# GitHub Pages 名刺・開業準備LPページ

中小企業の経理フロー改善・AI活用支援のための静的HTML名刺ページおよび開業準備LPです。

## 公開情報

- **公開URL（名刺）**: https://chuoline.github.io/
- **公開URL（開業準備LP）**: https://chuoline.github.io/lp/
- **リポジトリ**: https://github.com/chuoline/chuoline.github.io

## ファイル構成

```
/
├── index.html      # オンライン名刺（トップページ）
├── style.css       # 共通スタイル
├── lp/
│   └── index.html  # 開業準備LP
└── README.md
```

## 更新手順

内容を変更した場合は、**必ず作業ブランチで変更し、mainへのマージは人間の確認後に行うこと**。

```bash
cd ~/agent-system/github-pages
git checkout -b feature/your-change
# 変更作業
git add index.html style.css lp/index.html
git commit -m "変更内容の説明"
git push -u origin feature/your-change
# → GitHub上でPRを作成 or mainへマージ承認後に push origin main
```

mainへpushすると数分で反映される。

## ロールバック方法

```bash
# 直前のコミットを打ち消す（履歴を残すrevert）
cd ~/agent-system/github-pages
git revert HEAD
git push origin main
```

`git reset --hard` および `push --force` は、理由を説明し本人の明示承認を得た場合のみ使用する。

## コード正本の原則

- **公開サイトのHTML/CSS/画像の正本はこのリポジトリ**
- `agent-system/` 側には公開コードのコピーを置かない
- `agent-system/ai_handoff/` には要件・依頼書・決定事項・完了記録を保存する
