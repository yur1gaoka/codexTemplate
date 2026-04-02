# Codex Template Repository

Codex を使った開発やレビューのための、汎用ドキュメントテンプレートです。

## 目的

- 作業開始前に確認すべき条件を揃える
- 実装、調査、レビュー、文書更新を同じ枠組みで扱う
- 未確定情報を推測で埋めず、安全に引き継げる状態を保つ

## 前提

- 詳細な作業ルールは [AGENTS.md](./AGENTS.md) と `docs/` 配下の文書を基準にする
- テンプレート上の記述は汎用性を優先し、具体値は各プロジェクトで記入する
- 未確定の項目は空欄放置ではなく、`未確認` `確認待ち` `該当なし` を使い分ける

## 構成

- [AGENTS.md](./AGENTS.md): リポジトリ全体の作業ルール
- [docs/start.md](./docs/start.md): 作業開始手順
- [docs/project-profile.md](./docs/project-profile.md): プロジェクト条件の整理
- [docs/rules.md](./docs/rules.md): 絶対ルールと停止条件
- [docs/workflow.md](./docs/workflow.md): 作業方式と進め方
- [docs/output.md](./docs/output.md): 出力順序
- [docs/tasks.md](./docs/tasks.md): タスク定義の必須項目
- [docs/done.md](./docs/done.md): 完了条件
- [docs/commit.md](./docs/commit.md): コミットルール
- [docs/handover.md](./docs/handover.md): 継続作業時の引き継ぎ
- [docs/intake.md](./docs/intake.md): 条件確認
- [docs/code_review.md](./docs/code_review.md): レビュー観点
- [docs/structure.md](./docs/structure.md): 実装方針

## 使い方

1. [docs/start.md](./docs/start.md) から読み始める
2. [docs/project-profile.md](./docs/project-profile.md) に確認済み条件を記入する
3. [docs/tasks.md](./docs/tasks.md) に沿って作業種別と期待成果物を明確にする
4. [docs/workflow.md](./docs/workflow.md) に沿って、実装、調査、レビュー、文書更新のいずれかを進める
5. [docs/done.md](./docs/done.md) で完了条件を確認する
6. 継続作業がある場合は [docs/handover.md](./docs/handover.md) を更新する

## 運用メモ

- worktree は必要な場合のみ使う
- worktree を使う場合は、`./[プロジェクト名]/worktrees/[作業ブランチ名]` のような構成を想定する
- レビューや調査だけの作業は、実装タスクと分けて扱う
- README は概要、詳細は `AGENTS.md` と `docs/` に集約する

## 保護対象の扱い

- README などのユーザー向け文書では、作者メッセージ、クレジット、ライセンス表記を保護対象として扱う
- 明示的なユーザー指示または管理者指示がない限り、保護対象の削除・要約・書き換えは禁止
- 文書整備、同期、要約、リライト時も保護対象の文言を維持する
- 保護対象を変更する場合は、事前確認を必須とする

```md
<!-- 保護領域: 作者メッセージ。明示指示なしで削除・要約・書き換え禁止 -->
ここに作者メッセージ

<!-- 保護領域: クレジット表記。明示指示なしで削除・要約・書き換え禁止 -->
ここにクレジット表記

<!-- 保護領域: ライセンス表記。明示指示なしで削除・要約・書き換え禁止 -->
ここにライセンス表記
```
