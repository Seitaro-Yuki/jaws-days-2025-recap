---
marp: true
paginate: true
theme: kdx
style: |
  /* ここに CSS を記述します */
  section.lead h1 {
    text-align: center;
    font-size: 3em;
  }
  section.lead p {
    text-align: center;
    font-size: 1em;
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
