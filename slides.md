---
theme: seriph
colorSchema: dark
layout: intro
highlighter: shiki
download: true        # ← PDF出力を有効化
routerMode: hash      # ← Vercel 上でのルーティング不具合防止
---

# AIワークフローツール最新情報比較

Dify vs n8n vs SimAI

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/your-repo" target="_blank" alt="GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---
layout: default
---

# AIワークフローツールとは？

<div class="grid grid-cols-2 gap-12 items-center">
<div>

AIを組み込んだタスクやプロセスを自動化・効率化するためのツールです。

<br>

- 🤖 **LLM統合**: GPT等をワークフローに組み込む
- 🎨 **ノーコード/ローコード**: GUIでプロセスを構築
- 🔗 **外部サービス連携**: APIやSaaSと連携
- 📚 **RAG**: 独自データでAIの回答精度を向上

</div>
<div class="p-4 bg-gray-400/10 rounded-lg">
<img src="https://images.unsplash.com/photo-1678483749015-a6d5cfc7a3f2?q=80&w=2070&auto=format&fit=crop" class="rounded-lg shadow-lg">
<p class="text-xs text-center opacity-50 mt-2">A conceptual image of an automated workflow</p>
</div>
</div>

---
layout: default
---

# 1. Dify
<p class="opacity-75 !-mt-2">LLMアプリケーション開発・運用プラットフォーム</p>

<div class="flex items-center gap-8 mt-4">
  <div class="w-2/3">
    <p>オープンソースのLLMOpsプラットフォーム。RAGやAgent機能を持つAIネイティブなアプリケーションを、ノーコードで迅速に構築・運用することに特化しています。</p>
    <ul class="mt-4 text-lg space-y-2">
      <li><span class="text-green-300">✅</span> <strong>特徴:</strong> ビジュアルWorkflow、RAGパイプライン、Agent機能</li>
      <li><span class="text-blue-300">🎯</span> <strong>得意領域:</strong> 高機能AIチャットボット、ナレッジ検索</li>
      <li><span class="text-purple-300">👥</span> <strong>ターゲット:</strong> AIアプリ開発者、スタートアップ</li>
    </ul>
  </div>
  <div class="w-1/3 p-4 bg-white rounded-lg">
    <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/dify.png" alt="Dify Logo" class="max-h-40 mx-auto">
  </div>
</div>

---
layout: default
---

# 2. n8n
<p class="opacity-75 !-mt-2">拡張性の高いワークフロー自動化ツール</p>

<div class="flex items-center gap-8 mt-4">
  <div class="w-2/3">
    <p>汎用的なワークフロー自動化ツール。数百の外部サービス連携（ノード）が強みで、既存の業務プロセスにAIを組み込むのに適しています。</p>
    <ul class="mt-4 text-lg space-y-2">
      <li><span class="text-green-300">✅</span> <strong>特徴:</strong> 豊富な連携ノード、ビジュアルエディタ、セルフホスト</li>
      <li><span class="text-blue-300">🎯</span> <strong>得意領域:</strong> 複数SaaS連携、業務自動化へのAI適用</li>
      <li><span class="text-purple-300">👥</span> <strong>ターゲット:</strong> 開発者、マーケター、業務改善担当者</li>
    </ul>
  </div>
  <div class="w-1/3 p-4 bg-white rounded-lg">
    <img src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/n8n.png" alt="n8n Logo" class="max-h-40 mx-auto">
  </div>
</div>

---
layout: default
---

# 3. SimAI
<p class="opacity-75 !-mt-2">産業・エンジニアリング向けAIプラットフォーム</p>

<div class="flex items-center gap-8 mt-4">
  <div class="w-2/3">
    <p>主に製造業やエンジニアリング分野で利用されるAIプラットフォーム。物理シミュレーションの高速化や、デジタルツインの構築、予知保全などに特化しています。</p>
    <ul class="mt-4 text-lg space-y-2">
      <li><span class="text-green-300">✅</span> <strong>特徴:</strong> 物理シミュレーションAI高速化、需要予測</li>
      <li><span class="text-blue-300">🎯</span> <strong>得意領域:</strong> 製品設計、製造プロセス最適化、デジタルツイン</li>
      <li><span class="text-purple-300">👥</span> <strong>ターゲット:</strong> エンジニア、研究開発者、製造業DX担当者</li>
    </ul>
  </div>
  <div class="w-1/3 p-4 bg-gray-400 bg-opacity-10 rounded-lg h-48 flex flex-col justify-center">
    <p class="text-7xl text-center font-bold">SimAI</p>
    <p class="text-center text-sm opacity-75">(by Ansys / Simovate)</p>
  </div>
</div>

---
layout: default
---

# 機能比較まとめ

| 観点 | Dify | n8n | SimAI |
|---|---|---|---|
| **主な用途** | LLMアプリ開発・運用 | 汎用的な業務自動化 | 産業・工学シミュレーション |
| **中心機能** | RAG, Agent, Workflow | 豊富な連携ノード | 物理シミュレーションAI |
| **ターゲット** | AI開発者 | 幅広いビジネスユーザー | エンジニア, 研究者 |
| **AIの役割** | アプリケーションの核 | ワークフローの部品 | シミュレーションの高速化 |
| **オープンソース** | <span class="text-green-400 font-bold text-xl">⭕️</span> | <span class="text-green-400 font-bold text-xl">⭕️</span> | <span class="text-red-400 font-bold text-xl">❌</span> |

---
layout: default
---

# 結論：どのツールを選ぶべきか？

<div v-click class="p-4 border border-gray-400/20 rounded-lg mb-4 bg-gray-400/10 transition hover:border-purple-400/60">
  <p class="text-2xl font-bold text-purple-300">Dify</p>
  <p class="text-lg opacity-90">AIネイティブなチャットアプリやエージェントを素早く作りたい場合に最適。</p>
</div>

<div v-click class="p-4 border border-gray-400/20 rounded-lg mb-4 bg-gray-400/10 transition hover:border-green-400/60">
  <p class="text-2xl font-bold text-green-300">n8n</p>
  <p class="text-lg opacity-90">既存の業務や複数のSaaSにAIを組み込んで自動化したい場合に最適。</p>
</div>

<div v-click class="p-4 border border-gray-400/20 rounded-lg mb-4 bg-gray-400/10 transition hover:border-blue-400/60">
  <p class="text-2xl font-bold text-blue-300">SimAI</p>
  <p class="text-lg opacity-90">製品開発や製造プロセスをAIで効率化・高度化したい場合に最適。</p>
</div>

---
layout: intro
---

# ご清聴ありがとうございました
