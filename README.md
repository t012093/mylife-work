# GitHub Projects と Actions による Issue 管理

このリポジトリは、GitHub Projects と Actions を使用して Issue の状態を自動的に管理・可視化するプロジェクトです。仕事、日常のルーティーン、エンジニアリングタスクを効率的に管理できます。

## 機能

### 自動管理機能
- Issue が作成されると自動的に「Backlog」列に追加
- 担当者がアサインされると自動的に「In Progress」列に移動
- Issue がクローズされると自動的に「Done」列に移動
- 各状態に応じて自動的にラベル（backlog/inprogress/close）を付与

### Issue テンプレート

#### 1. 仕事用テンプレート
- 業務カテゴリの選択（会議、資料作成、企画など）
- 優先度の設定
- 期限の指定
- 詳細な業務内容の記述

#### 2. ルーティーンタスク用テンプレート
- カテゴリ（健康管理、自己啓発、家事など）
- 実施頻度の設定
- 実施時間帯の指定
- 具体的な目標や準備物の記録

#### 3. エンジニアリング用テンプレート
- 開発カテゴリの選択
- 優先度の設定
- 関連コンポーネントの指定
- 技術的詳細の記述
- チェックリストによる進捗管理

## セットアップ

1. このリポジトリをクローン
2. GitHub Personal Access Token (PAT) を生成
   - Settings > Developer settings > Personal access tokens > Generate new token
   - 必要な権限: `repo` スコープ
3. リポジトリの Settings > Secrets に PAT を `KEY` という名前で追加
4. Projects タブでプロジェクトを作成
   - プロジェクト名を「mylife」に設定
   - 「Backlog」「In Progress」「Done」の3つの列を作成

## 使用方法

1. Issue の作成
   - 目的に応じて適切なテンプレートを選択
   - 必要な情報を入力
   - 自動的に「Backlog」列に追加

2. Issue の管理
   - 担当者をアサインすると「In Progress」に移動
   - 作業完了後にクローズすると「Done」に移動
   - 各状態に応じて自動的にラベルが更新

3. プロジェクトボードの活用
   - カテゴリ別の進捗確認
   - 優先度に基づくタスク管理
   - 期限管理による効率的な作業計画
