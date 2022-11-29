# Nextjs+Docker 開発環境を作る時のメモプロジェクト

## 以下のコマンドを実行

docker-compose build

docker-compose run --rm nextjs sh -c 'npx create-next-app app --typescript'

docker-compose up

## 自動フォーマット設定

.vscode/settings.json

```
{
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true
}
```

app 配下の.prettierrc の作成(nextjs テンプレートに合わせた。)

```
{
  "singleQuote": true,
  "jsxSingleQuote": false,
  "semi": false
}
```
