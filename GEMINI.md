
system_instruction:
  goal: "AIワークフローツールに関するSlidevプレゼンテーションを作成し、Vercelデプロイ設定を整える。具体的には、Dify, n8n, SimAIの3ツールを比較する`slides.md`、Slidevのビルド設定を含む`package.json`、Vercelのデプロイ設定である`vercel.json`を作成する。"
  files_to_create:
    - file_path: "slides.md"
      content: |
        ---
        theme: 'default'
        layout: 'intro'
        ---

        # AIワークフローツール最新情報比較

        Dify vs n8n vs SimAI

        ---
        layout: 'default'
        ---

        # AIワークフローツールとは？

        AIを組み込んだ一連のタスクやプロセスを自動化・効率化するためのツールです。

        - **LLM（大規模言語モデル）の統合**: GPTやClaudeなどのAIモデルをワークフローに組み込む。
        - **ノーコード/ローコード**: GUI上でドラッグ＆ドロップ操作により、複雑なプロセスを構築。
        - **外部サービス連携**: 様々なAPIやSaaSと連携し、データの入出力を自動化。
        - **RAG（検索拡張生成）**: 独自のデータソースをAIに連携させ、より正確な回答を生成。

        本日は、注目の3ツールを比較します。

        ---
        layout: 'default'
        ---

        # 1. Dify

        <div class="flex items-center">
          <div class="w-2/3">
            <p class="text-xl"><strong>LLMアプリケーション開発・運用プラットフォーム</strong></p>
            <p>オープンソースのLLMOpsプラットフォーム。RAGやAgent機能を持つAIネイティブなアプリケーションを、ノーコードで迅速に構築・運用することに特化しています。</p>
            <ul class="mt-4">
              <li>✅ <strong>主な特徴:</strong> ビジュアルなWorkflowビルダー、RAGパイプライン、Agent機能、豊富なモデルサポート</li>
              <li>✅ <strong>得意領域:</strong> 高機能なAIチャットボット、ナレッジベース検索、AIエージェントの開発</li>
              <li>✅ <strong>ターゲット:</strong> AIアプリケーション開発者、スタートアップ</li>
            </ul>
          </div>
          <div class="w-1/3 p-4">
            <img src="https://dify.ai/logo/logo-light.svg" alt="Dify Logo" class="max-h-40 mx-auto">
          </div>
        </div>

        ---
        layout: 'default'
        ---

        # 2. n8n

        <div class="flex items-center">
          <div class="w-2/3">
            <p class="text-xl"><strong>拡張性の高いワークフロー自動化ツール</strong></p>
            <p>汎用的なワークフロー自動化ツールですが、近年AI関連の機能を大幅に強化。数百の外部サービス連携（ノード）が強みで、既存の業務プロセスにAIを組み込むのに適しています。</p>
            <ul class="mt-4">
              <li>✅ <strong>主な特徴:</strong> 豊富な連携ノード、ビジュアルエディタ、セルフホスティング可能、AI関連ノード（LLM, Vector Store）</li>
              <li>✅ <strong>得意領域:</strong> 複数SaaSを連携させた業務自動化、定型業務へのAI適用</li>
              <li>✅ <strong>ターゲット:</strong> 開発者、マーケター、業務改善担当者</li>
            </ul>
          </div>
          <div class="w-1/3 p-4">
            <img src="https://n8n.io/n8n-logo.svg" alt="n8n Logo" class="max-h-40 mx-auto">
          </div>
        </div>

        ---
        layout: 'default'
        ---

        # 3. SimAI

        <div class="flex items-center">
          <div class="w-2/3">
            <p class="text-xl"><strong>産業・エンジニアリング向けAIプラットフォーム</strong></p>
            <p>主に製造業やエンジニアリング分野で利用されるAIプラットフォーム。物理シミュレーションの高速化や、デジタルツインの構築、予知保全などに特化しており、汎用ツールとは一線を画します。</p>
            <ul class="mt-4">
              <li>✅ <strong>主な特徴:</strong> 物理シミュレーションのAIによる高速化、需要予測、予知保全</li>
              <li>✅ <strong>得意領域:</strong> 製品設計、製造プロセス最適化、デジタルツイン</li>
              <li>✅ <strong>ターゲット:</strong> エンジニア、研究開発者、製造業のDX担当者</li>
            </ul>
          </div>
          <div class="w-1/3 p-4">
            <p class="text-6xl text-center font-bold">SimAI</p>
            <p class="text-center text-sm">(by Ansys / Simovate)</p>
          </div>
        </div>

        ---
        layout: 'default'
        ---

        # 機能比較まとめ

        | 観点 | Dify | n8n | SimAI |
        |---|---|---|---|
        | **主な用途** | LLMアプリ開発・運用 | 汎用的な業務自動化 | 産業・工学シミュレーション |
        | **中心機能** | RAG, Agent, Workflow | 豊富な連携ノード | 物理シミュレーションAI |
        | **ターゲット** | AI開発者 | 幅広いビジネスユーザー | エンジニア, 研究者 |
        | **AIの役割** | アプリケーションの核 | ワークフローの部品 | シミュレーションの高速化 |
        | **オープンソース** | ⭕️ | ⭕️ | ❌ |

        ---
        layout: 'default'
        ---

        # 結論：どのツールを選ぶべきか？

        - **AIネイティブなチャットアプリやエージェントを素早く作りたい**
          - 👉 **Dify** が最適

        - **既存の業務や複数のSaaSにAIを組み込んで自動化したい**
          - 👉 **n8n** が最適

        - **製品開発や製造プロセスをAIで効率化・高度化したい**
          - 👉 **SimAI** が最適

        ---
        layout: 'intro'
        ---

        # ご清聴ありがとうございました
    - file_path: "package.json"
      content: |
        {
          "name": "ai-workflow-slides",
          "private": true,
          "scripts": {
            "build": "slidev build --base /",
            "dev": "slidev",
            "export": "slidev export"
          },
          "dependencies": {
            "@slidev/cli": "^0.49.0",
            "@slidev/theme-default": "^0.25.0"
          }
        }
    - file_path: "vercel.json"
      content: |
        {
          "buildCommand": "npm run build",
          "outputDirectory": "dist"
        }
