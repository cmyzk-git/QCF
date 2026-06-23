# QCF v1.0 Draft

Qcard Content Format

Version: 1.0 Draft

Status: Proposal

Project: G.E.D.A. (Global Existential Deep Archive)

---

# 1. Purpose

QCF（Qcard Content Format）は、知識コンテンツを保存・共有・学習・販売するための標準フォーマットである。

QCFは特定のアプリケーションに依存しない。

QCFで記述されたコンテンツは、Qcard、GEDA、AIシステム、および将来の外部サービス間で相互利用できることを目的とする。

---

# 2. Design Principles

## Human First

人間が読めること。

QCFは機械可読性だけでなく、人間が直接編集できることを重視する。

---

## AI Native

AIが生成・編集しやすいこと。

Claude、ChatGPT、Geminiなどが自然に出力可能な構造とする。

---

## Portable

特定サービスに依存しない。

QCFデータは環境を問わず移行できること。

---

## Long-term Archive

長期保存を前提とする。

10年後でも内容を理解できる構造を目指す。

---

# 3. Content Model

QCFは以下の階層で構成される。

Collection

↓

Deck

↓

Card

---

## Collection

コンテンツの集合。

例：

* 広告業界面接対策
* 日本史
* 英会話
* GEDA感覚辞典

---

## Deck

テーマ単位のまとまり。

例：

* 志望動機
* 強み
* 弱み
* キャリア

---

## Card

最小学習単位。

QCFの基本構造。

---

# 4. Card Structure

Cardは以下の情報を持つ。

Required

* id
* question
* answer

Optional

* hint
* tags
* source
* notes
* audio
* metadata

---

## Example

Question

「あなたの強みは？」

Answer

「課題発見力です。」

Hint

「具体的なエピソードを添える」

Tags

* 面接
* 自己PR

---

# 5. Metadata

QCFは以下のメタデータを保持できる。

* title
* author
* version
* language
* created_at
* updated_at
* license

---

Example

title:
広告業界面接対策

author:
GEDA

language:
ja

version:
1.0

---

# 6. Content Types

QCFは複数のコンテンツタイプを扱う。

## Study

一般学習

---

## Interview

面接練習

---

## Language

語学学習

---

## Presentation

プレゼン練習

---

## Sales

営業ロープレ

---

## Reading

朗読練習

---

## GEDA

概念・感覚アーカイブ

---

# 7. Audio Support

Cardは音声データを保持できる。

対象：

* TTS音声
* ユーザー録音
* 発音サンプル

音声形式は実装依存とする。

---

# 8. AI Compatibility

QCFはAIとの連携を前提とする。

AIは以下を実行できる。

* QCF生成
* QCF編集
* QCF変換
* QCF要約
* QCF分類

---

# 9. Marketplace Compatibility

QCFは将来的なコンテンツ販売を想定する。

販売対象はQCFコンテンツそのものである。

販売者は著作権を保持する。

プラットフォームは利用ライセンスを提供する。

---

# 10. Relationship to GEDA

GEDAは知識と概念を発見・記録するプロジェクトである。

QCFはGEDAにおける知識保存規格である。

QcardはQCFを学習するためのアプリケーションである。

Relationship

GEDA
↓
QCF
↓
Qcard

---

# 11. Future Extensions

将来的に以下の拡張を予定する。

* 評価スコア
* 学習履歴
* 習熟度
* AIフィードバック
* 音声解析
* 共同編集
* マーケットプレイス連携

---

# 12. Versioning

フォーマットの互換性維持のため、Semantic Versioningを採用する。

Examples

1.0.0

1.1.0

2.0.0

---

End of Specification
