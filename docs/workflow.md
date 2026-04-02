# workflow.md

## 開発方式
司令官方式で進める

## ブランチとworktreeの関係（重要）

- ブランチ：履歴の分岐
- worktree：作業フォルダ

関係：
- 1ブランチ = 1worktree に対応させる

## フォルダ構成

C:\test
├─ main                  ← mainブランチ
└─ worktrees
   ├─ feature-ui         ← feature/ui ブランチ
   ├─ feature-sound      ← feature/sound ブランチ
   └─ ...

## 役割

### 司令官（main）
- タスク分割
- 指示生成
- レビュー
- 統合
- 実装禁止

### 作業者（各worktree）
- 指定範囲のみ変更
- 他領域変更禁止

## 原則
- 1スレッド1責務
- 1スレッド1worktree
- 差分変更のみ

## worktree運用
- 初期は main のみ使用
- 並列作業時のみ worktree を作成
- 各 worktree は専用ブランチに紐付ける

## 統合
- main にマージする
- 統合は司令官のみ実施
- 作業スレッドは統合禁止

## 禁止
- 同一フォルダで複数ブランチを切り替えて作業すること
- 複数スレッドで同一ファイルを編集すること