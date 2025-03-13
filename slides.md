---
marp: true
paginate: true
theme: kdx
style: |
  /* ここに CSS を記述します */
  section.lead h1 {
    text-align: start;
    font-size: 4em;
  }
---

<!--
_class: lead
_paginate: false
-->

# JAWS DAYS 2025 Recap

クラウドサービス部
結城清太郎

---

# 概要

- 公式サイト: https://jawsdays2025.jaws-ug.jp/
- 開催日: 2025年3月1日(土)
- 会場: サンシャインシティ 展示ホールA
- テーマ: connecting the dots - 繋がりから生まれる新たなイノベーション
- JAWS DAYSの魅力
  - 最新技術動向や活用事例を学べる
  - 他のユーザーと交流できる
  - JAWS-UGメンバーが主体となって運営
  - AWSのスキルアップ、人脈形成、情報収集

---

# IAMのマニアックな話2025

- セッション: https://jawsdays2025.jaws-ug.jp/sessions/A-1
- スライド: https://speakerdeck.com/nrinetcom/iamnomaniatukunahua-2025
- 2019年に https://booth.pm/ja/items/1563844 という本を出した著者が今年新しい本を出すにあたって2019年からのIAM周りの変化を説明する

---

# IAMのマニアックな話2025

- **2019年からの変化**:
  - IAMユーザー中心から**IAM Identity Centerを活用しゼロへ** 
  - 明示的なポリシー定義から **動的制御（ABAC）+ 組織制御（SCP/RCP）** へ 
  - 定期監査から**リアルタイム監査（IAM Access Analyzer）+ AI提案**へ 
- **主要なアップデートと状況の変化**:
  - **IAM Access Analyzer**による問題設定の自動検出
  - **ABAC**（属性ベースアクセス制御）の一般化による柔軟な権限管理
  - **RCP**（リソースコントロールポリシー）による組織全体でのリソース制御
  - **AWS Verified Access**による動的なアクセス許可とゼロトラスト対応
  - **IAM Identity Center**とAWS Organizationsの統合強化

---

# IAMのマニアックな話2025

- **これからのベストプラクティス**:
  - **IAMユーザーは原則利用せず、IAM Identity Centerを活用** 
  - **ABACとSCP/RCPを組み合わせた多層的なポリシー設計** 
  - **IAM Access Analyzerによる継続的な監査と改善** 
  - **AWS Verified Accessなどを活用したゼロトラストアーキテクチャ** 
- **認証認可管理の課題**: IdP、IAM Identity Center、各アカウントのIAMロールの管理主体の連携 
- **今後のトレンド予想**:
  - ゼロトラストIAMへの移行とAWS Verified Accessの統合 
  - AIによるポリシー推奨・自動生成 
  - 動的なIAM管理の標準化とアクセス管理の自動化 
    
---

## IAMの変遷と今後の展望

- **2019年から2025年でIAMのベストプラクティスは大きく変化**しました [1]。
- **IAMユーザーの運用方針**: 最小限からIAM Identity Centerを活用したゼロへ [2, 3]。
- **IAMポリシーの設計**: 明示的な定義から、動的な制御（ABAC）と組織制御（SCP/RCP）による最適化へ [4-8]。
- **監査の強化**: 定期監査からIAM Access Analyzerによるリアルタイム監査とAI提案へ [9, 10]。

---

# IAMのマニアックな話2025

## 主要なIAMコンセプトとテクノロジー

- **属性ベースのアクセス制御（ABAC）**: プリンシパルとリソースの属性（タグ）に基づいたきめ細かいアクセス制御 [6, 7, 11]。**ポリシーの簡略化と動的な管理**が期待されます [11]。
- **リソースコントロールポリシー（RCP）**: AWS Organizationsの機能として登場。組織全体でリソース単位のアクセス制御を適用 [6, 8]。
- **AWS Verified Access**: VPNに代わる、**リクエスト評価に基づいた動的なアクセス許可**の仕組み。IdPと連携し、ゼロトラストを実現 [6]。
- **IAM Access Analyzer**: 外部アクセス、未使用アクセスを分析し、**問題のある設定を自動検出**。CloudTrailログからのポリシー生成も可能 [6, 9, 10]。

---

# IAMのマニアックな話2025

## 今後のIAMトレンドと課題

- **ゼロトラストIAMへの移行**: AWS Verified Accessなどの活用により、よりセキュアなアクセス制御へ 。
- **AIによるポリシー推奨・自動生成**: IAM Access Analyzerの進化により、**効率的な権限管理**が期待されます [10]。
- **動的なIAM管理とアクセス管理の自動化**: ABACなどの技術により、**柔軟かつ効率的なアクセス管理**が標準化へ [11]。
- **管理主体の分散**: IdP、IAM Identity Center、各アカウントのIAMロールの管理を組織全体でどう連携させるかが課題 。
- **全体像の把握**: 変化の激しいIAM関連サービスを「点と点を結びつけて全体像を把握する」ことの重要性 [8]。
