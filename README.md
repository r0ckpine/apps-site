# apps-site

HoverTick のプライバシーポリシー・サポートページを公開するGitHub Pagesサイトです。
This repository hosts the privacy policy and support pages for HoverTick.

## 公開手順

1. このリポジトリ(`r0ckpine/apps-site`)を **Public** にする(無料プランのGitHub Pagesには必須)
2. 中身一式を `main` ブランチにpush
3. Settings → Pages → Source: `main` branch / `(root)` → Save
4. 数分後、以下のURLが有効になります

## App Store Connect 登録用URL

| App | Privacy Policy | Support |
|---|---|---|
| HoverTick | `https://r0ckpine.github.io/apps-site/hovertick/privacy` | `https://r0ckpine.github.io/apps-site/hovertick/support` |

プライバシーポリシーのURLはアプリ内(`HoverTick/AppLinks.swift`)にも埋め込まれています。パスを変える場合はアプリ側も合わせて更新してください。

## 新しいアプリを追加する場合

1. ルートに新しいディレクトリを作成(例: `newapp/`)
2. `hovertick/privacy.md` `hovertick/support.md` をコピーして中身を書き換え
3. `index.md` にリンクを追加
