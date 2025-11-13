# try_claude

AI(Claude)との対話を GitHub 上で直接行えるリポジトリです。`@claude`メンションでClaudeを呼び出せます。

## 🤖 特徴

- **GitHub上で直接対話**: Issue/PRで`@claude`とメンションするだけ
- **コード実装**: Claudeがコードの実装・修正を支援
- **レビュー**: 自動的にコードレビューを実施
- **ドキュメント生成**: 指示に従ってドキュメントを作成

## 🚀 使い方

### 1. Issueで質問

Issue内で`@claude`をメンションして質問:
```markdown
@claude このプロジェクトのREADMEを作成してください。

以下の内容を含めてください:
- プロジェクト概要
- セットアップ手順
- 基本的な使い方
```

### 2. PRでレビュー依頼

PRのコメントで:
```markdown
@claude このPRをレビューしてください。

特に以下の点を確認してください:
- コードの品質
- ドキュメントの分かりやすさ
```

### 3. コード実装の依頼
```markdown
@claude 以下の機能を実装してください:

- テストファイルの作成
- エラーハンドリングの追加
```

## 📂 ディレクトリ構成
```
try_claude/
├── .github/
│   ├── workflows/
│   │   └── claude.yml                  # Claude GitHub Action
│   ├── ISSUE_TEMPLATE/
│   │   └── ai_discussion.md            # AI用テンプレート
│   └── PULL_REQUEST_TEMPLATE.md        # PR テンプレート
├── docs/
│   └── github-discussion-prompts.md    # プロンプト集
├── CLAUDE.md                            # Claudeへの指示
└── README.md
```

## 💡 Tips

### 効果的な質問の仕方

1. **具体的に**: 「このコードをレビューして」より「このコードのパフォーマンスを改善してください」
2. **コンテキストを提供**: 背景情報を含める
3. **期待する形式を明示**: 箇条書き、コードブロックなど

### ワークフロー

1. **Issue作成** → `@claude`で質問・相談
2. **ブランチ作成** → 開発
3. **PR作成** → `@claude`でレビュー依頼
4. **修正** → `@claude`と協力して改善
5. **マージ**

## 📚 参考資料

- [プロンプト集](docs/github-discussion-prompts.md)
- [Claude Code Action](https://github.com/anthropics/claude-code-action)
- [GitHub Flow](https://docs.github.com/ja/get-started/quickstart/github-flow)

## 🤝 コントリビューション

Issue や Pull Request を歓迎します!`@claude`を活用してください。

---

**作成日**: 2025-11-13  
**メンテナ**: @FT-FumihikoUnno
