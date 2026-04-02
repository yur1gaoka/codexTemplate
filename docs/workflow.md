# workflow.md

## 開発方式
司令官方式

---

## ブランチとworktree（明確化）

- ブランチ：履歴の分岐
- worktree：作業フォルダ

関係：
1ブランチ = 1worktree

---

## フォルダ構成

C:\test
├─ main
└─ worktrees
   ├─ feature-a
   ├─ feature-b
   └─ ...

---

## 役割

### 司令官（main）
- タスク分割
- 条件確認
- レビュー
- 統合
- 実装禁止

### 作業者（worktree）
- 指定範囲のみ変更

---

## 作業フロー（強制）

1. start.md を読む
2. intake.md で条件確認（必要時）
3. project-profile.md を確認・更新
4. handover.md を確認
5. tasks.md に従いタスク確認
6. 小さい計画提示
7. 実装
8. done.md に基づき確認
9. commit.md に従いコミット
10. handover.md 更新

---

## 統合

- main にマージ
- 司令官のみ実施

---

## 禁止

- 同一フォルダで複数ブランチ作業
- handover未更新で終了
- done未確認で完了