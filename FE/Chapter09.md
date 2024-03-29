## 9-1 情報システム戦略とシステム企画 ◎
- 情報システム戦略
  - **全体最適化計画**：全社的な観点から情報システムのあるべき姿を明確にする計画
  - 情報システム管理基準：情報システムの管理を効果的に行うための実践規範を、経済産業省が体系的にまとめたもの
  - CIO（Chief Information Officer）：全社的な観点から情報戦略を立案し、経営戦略との整合性の確認・評価を行う役員
  - **ITガバナンス**：情報システム戦略の策定と実行をコントロールする組織の能力のこと
- **エンタープライズアーキテクチャ**（EA）：各業務と情報システムを、全体最適化の観点から見直すための技法
  - ビジネスアーキテクチャ
  - データアーキテクチャ
  - アプリケーションアーキテクチャ
  - テクノロジーアーキテクチャ
- **共通フレーム**（共通フレーム2013）：ソフトウェア開発作業全般にわたって「共通の物差し」となるガイドライン
- 企画プロセス
  - システム化構想：経営事業の目的・目標を達成するために、経営上のニーズと課題を確認し、経営戦略に基づいたシステム化の方針を立案すること
  - **システム化計画**：システム化構想を具現化するために立案する計画
- **要件定義プロセス**：利用者のニーズを整理し、新たに構築する（再構築する）業務とシステムの仕様や範囲を明らかにして、利害関係者間で合意します
  - 業務要件
  - 機能要件
  - **非機能要件**
- 調達計画・実施
  - **情報提供依頼**：ベンダ企業に対して、システム化の目的や業務内容などを示し、利用可能な技術や製品、導入実績などの実現手段に関する情報提供を依頼すること
  - **提案依頼書**：ベンダ企業に対して、対象システムや調達条件などを示し、提案書の提出を依頼する文書
  - 提案書：ベンダ企業がRFPを基に開発体制やシステム構成、開発手法などを検討し、提案する文書
  - 見積書：ベンダ企業がシステムの開発や運用、保守などにかかる費用を提示する文書
  - NDA：秘密保持契約
  - CSR：企業が本来の営利活動とは別に、社会の一員として社会的責任を果たすこと
    - **グリーン購入**：グリーンITを実施している製品・サービスを選ぶこと


> 「情報システム戦略」とくれば「経営戦略に基づいた情報システムを活用した戦略」

> 「RFI」とくれば「ベンダ企業に対して、情報提供を依頼すること」
> 
> 「RFP」とくれば「ベンダ企業に対して、提案書の提出を依頼する文書」

## 9-2 ソフトウェア開発 ◎
- ソフトウェア開発工程
  1. システム要件定義
  2. ソフトウェア要件定義
  3. システム設計
  4. ソフトウェア設計
  5. 実装・構築
  6. テスト
- ソフトウェア開発手法
  - **ウォーターフォールモデル**：上位工程から下位工程へ順番に進めていく開発手法
  - **アジャイル開発**：「短いサイクルで動作するプログラムを作成する」という作業を繰り返し、変化の激しい経営環境や利用者の要件を随時取り入れながら、段階的にシステム全体を完成させていく開発手法
    - **XP（エクストリームプログラミング）**：
      - イテレーションと呼ばれる短いサイクル（１〜２週間）で、動作するプログラムを作成する。
      - ２人一組になってプログラミングをする（ペアプログラミング）。
      - 外部仕様を変更することなく、プログラム内部構造を変更する。（リファクタリング）
      - 継続的インテグレーション
      - テストファースト
    - スクラム開発
      - スプリントと呼ばれる短いサイクル（１〜４週間）動作するプログラムを作成する。
      - 毎日のミーティング（デイリースクラム）を実施。
  - プロトタイピングモデル：システム開発の早い段階から試作品（プロトタイプ）を作成して、利用者の確認を得ながら開発を進めていく開発手法。
  - スパイラルモデル：システムをさらに独立性の高いサブシステムに分割し、サブシステムごとに要件定義や設計、開発、テストを繰り返しながら段階的にシステムを完成させていく開発手法。
  - **リバースエンジニアリング**：既存のプログラムを解析して、プログラムの仕様と設計書を取り出す開発手法。
  - DevOps：開発部門と運用部門が緊密に連携してシステムの改善を進めようという考え方。
  - CMMI（統合能力成熟度モデル）：システム開発組織におけるプロセス成熟度を評価するモデル。

> 「ウォータフォールモデル」とくれば「上位工程から下位工程へ順番に進める」
> 
> 「アジャイル開発」とくれば「短いサイクルで、動作するプログラムを作成する。を繰り返す」
