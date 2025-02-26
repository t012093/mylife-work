# GitHub Projects と Actions による Issue 管理

このリポジトリは、GitHub Projects と Actions を使用して Issue の状態を自動的に管理・可視化するデモプロジェクトです。

## 機能

- Issue が作成されると自動的に「Backlog」列に追加
- 担当者がアサインされると自動的に「In Progress」列に移動
- Issue がクローズされると自動的に「Done」列に移動
- 各状態に応じて自動的にラベル（backlog/inprogress/close）を付与
- プリオリティ管理機能
  - Daily（毎日対応）: `priority:daily`ラベル
  - Weekly（週次対応）: `priority:weekly`ラベル
  - Issue作成時にテンプレートから優先度を選択可能

## セットアップ

1. このリポジトリをクローン
2. GitHub Personal Access Token (PAT) を生成
   - Settings > Developer settings > Personal access tokens > Generate new token
   - 必要な権限: `repo` スコープ
3. リポジトリの Settings > Secrets に PAT を `PAT` という名前で追加
4. Projects タブでプロジェクトを作成
   - プロジェクト名を「test」に設定
   - 「Backlog」「In Progress」「Done」の3つの列を作成

## 使用方法

1. Issue を作成すると自動的に「Backlog」列に追加される
2. Issue に担当者をアサインすると「In Progress」列に移動
3. Issue をクローズすると「Done」列に移動
