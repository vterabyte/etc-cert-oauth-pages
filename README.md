# etc-cert-oauth-pages

`cloud-jobs/etc-cert`(ETC利用証明書の Google ドライブ自動保管)が使う Google OAuth 同意画面のための公開ページ。
GCP 同意画面を「本番」に公開するには、承認済みドメイン上のホームページ URL とプライバシーポリシー URL が必須
(2026-10-28 に判明)なので、このリポジトリだけ **意図的に Public** にして GitHub Pages で配信している。

- ホームページ: https://vterabyte.github.io/etc-cert-oauth-pages/
- プライバシーポリシー: https://vterabyte.github.io/etc-cert-oauth-pages/privacy.html
- GCP プロジェクト: temporal-frame-446907-k3(Google Auth Platform → ブランディング に上記 URL を登録)

## ルール

- 個人情報・認証情報・業務データを **絶対に置かない**(Public のため)
- ページの文言を変えるときは、アプリの実際の挙動(自分のドライブに PDF と台帳を保存するだけ)と一致させる
- `git push origin main` で GitHub Pages が自動デプロイ(約 1 分)
