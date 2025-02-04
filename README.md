# GitHub Repository Search - コンフリクト解決練習 🔄

このプロジェクトは、GitHubのリポジトリ検索機能を実装しながら、実践的なコンフリクト解決を学ぶための練習用リポジトリです。

## 🎯 目的

- Gitの基本操作の習得
- コンフリクトの解決方法の理解
- チームでのコードレビューの練習
- プルリクエストの作成と対応の練習

## 💻 開発環境

- Node.js 18以上
- Next.js 14
- TypeScript
- TailwindCSS

## 🚀 セットアップ手順

```bash
# リポジトリのクローン
git clone https://github.com/junjun-1345/team-dev-learn.git

# 依存関係のインストール
npm install

# 開発サーバーの起動
npm run dev
```

## 👥 チーム分け

AチームとBチームに分かれて作業を行います。各チームは同じファイルの同じ箇所を異なる方法で修正します。

### Aチームの担当
- リポジトリカード（青系デザイン）
- スター数表示（青系デザイン）
- 検索ボタン（青系デザイン）

### Bチームの担当
- リポジトリカード（グレー系デザイン）
- スター数表示（緑系デザイン）
- 検索ボタン（緑系デザイン）

## 📝 作業の進め方

1. **ブランチの作成**
```bash
git checkout -b feature/issue_99
```
feature/issue_<イシューの番号>

2. **作業とコミット**
```bash
# 変更を追加
git add .

# コミット
git commit -m "変更の説明"

# プッシュ
git push origin feature/[チーム名]/card-design
```

3. **プルリクエストの作成**
- GitHubで自分のブランチからmainブランチへのプルリクエストを作成
- タイトルと説明を適切に記入
- レビュワーを指定

## 🔄 コンフリクト解決の手順

1. コンフリクトの確認
```bash
git pull origin main
```

2. コンフリクトの解決
- コンフリクトが発生しているファイルを確認
- チーム間で相談して最適な解決方法を決定
- コードを適切に修正

3. 解決後のコミット
```bash
git add .
git commit -m "コンフリクトを解決"
git push origin feature/[チーム名]/card-design
```

## ✅ コードレビューのポイント

- デザインの一貫性
- コードの可読性
- コンポーネントの再利用性
- アクセシビリティ
- レスポンシブ対応

## 🎨 デザインガイドライン

### Aチームのデザイン
```css
/* カードのスタイル */
bg-gradient-to-r from-blue-50 to-blue-100
rounded-xl
shadow-md
hover:-translate-y-1

/* テキストカラー */
text-blue-600
font-bold
```

### Bチームのデザイン
```css
/* カードのスタイル */
bg-gray-50
rounded-md
shadow-sm
hover:bg-gray-100

/* テキストカラー */
text-green-600
font-semibold
```

## 📊 進捗管理

1. Issueのステータス
- 未着手 → 作業中 → レビュー待ち → 完了

2. プルリクエストのステータス
- レビュー待ち → レビュー中 → 変更リクエスト → 承認済み

## 🤝 コミュニケーション

- Issueでの議論
- プルリクエストでのコードレビュー
- コンフリクト発生時は必ずチーム間で相談

## ⭐ 練習のポイント

1. **ブランチ戦略**
- 機能ごとにブランチを作成
- こまめにコミット
- 定期的にmainブランチの変更を取り込む

2. **コミットメッセージ**
```
feat: 検索ボタンのデザインを変更
fix: カードのホバーアニメーションを修正
style: スター数の表示を改善
```

3. **コンフリクト解決のコツ**
- 相手の変更内容を理解する
- チームで相談して最適な解決方法を決める
- 必要に応じて両方のデザインを活かす方法を考える

## 📝 練習の進め方

1. まずIssueを確認してタスクを理解
2. 作業ブランチを作成して実装開始
3. こまめにコミットしながら作業
4. プルリクエストを作成
5. コンフリクトが発生したら解決
6. レビューとマージ

## 🚫 よくある間違い

- mainブランチで直接作業
- コミットメッセージが不明確
- コンフリクト解決時に相談なしで進める
- レビューを待たずにマージ

このREADMEを参考に、効果的なチーム開発の練習を行ってください。不明点があればIssueで質問してください！
