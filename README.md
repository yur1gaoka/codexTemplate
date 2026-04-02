# Template Repository

Codex運用テンプレート

## 特徴
- 司令官方式
- doc駆動
- 差分変更
- 並列作業対応

## ブランチとworktree

- ブランチ：履歴の分岐
- worktree：作業フォルダ

1ブランチ = 1worktree で運用する

## 構成

C:\test
├─ main
└─ worktrees

## 使い方

1. 条件確認
2. 設計
3. 実装
4. 要約

## 並列作業

- 必要時のみ worktree を作る
- 各作業は別フォルダで行う
- main で統合する