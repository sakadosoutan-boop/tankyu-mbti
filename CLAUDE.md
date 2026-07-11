# CLAUDE.md

探究MBTI — 90問の質問に答えることで、人文・社会/理工・自然/現代・国際/地域・生活の16系統の中から、自分が本当に関心を持っている探究テーマを発見できる診断クイズアプリ。

## 構成
- index.html 単一ファイル（1422行、HTML/CSS/JSを内包）。外部依存を増やさない方針。

## 公開
- 公開URL: https://sakadosoutan-boop.github.io/tankyu-mbti/
- mainブランチへのpushでGitHub Pagesに公開される。

## 編集ルール
- 変更は index.html 単一ファイル内で完結させる。
- 大きな変更前にファイル全体の構造（style/scriptブロックの区切り）を確認する。

## コミット規約
- 「Update index.html」のような曖昧なメッセージは避け、feat:/fix:/docs:/chore: ＋日本語要約でコミットする。

## モデル/トークン運用（標準指示）
- この規模のリポジトリの編集は Sonnet 以下のモデルで十分。
- オーケストレーター本体のトークン消費を抑えるため、探索はSonnet、実装はOpusのサブエージェントに委譲するのを標準とする。
