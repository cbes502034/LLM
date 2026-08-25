# AI 橋接手冊

從後端工程師轉職 AI 工程師的面試導向學習教材。以「這個 IP／這篇留言是不是威脅？」這個貫穿案例（延伸自 Threat Intel Agent 專案的真實資料），串連機器學習 → 深度學習 → LLM 三個階段，共九個模組，每個模組都是一個獨立的自足 HTML 檔案。

## 怎麼看

直接下載對應的 `.html` 檔案，用瀏覽器開啟即可（每個檔案都是 self-contained，不需要額外的伺服器或依賴）。也可以開啟 GitHub Pages，把 `index.html` 當作首頁。

## 模組列表

| 模組 | 標題 | 主題 | 分級 |
|---|---|---|---|
| [總覽](index.html) | AI橋接手冊 | 框架說明、學習路線圖、模組地圖 | — |
| M1 | [分類判官](module-m1-classification.html) | 分類問題、資料切分、混淆矩陣與評估指標 | 必修 |
| M2 | [決策森林](module-m2-decision-trees.html) | 決策樹（資訊獲利／Gini）→ 隨機森林 → AdaBoost | 必修 |
| M3 | [邊界與鄰居](module-m3-knn-svm-bayes.html) | KNN／SVM／貝氏分類器（概念層） | 選修・略讀 |
| M4 | [梯度引擎](module-m4-gradient-descent.html) | Tensor、梯度下降、Autograd 自動微分 | 必修 |
| M5 | [訓練迴圈](module-m5-training-loop.html) | nn.Module、Loss、Optimizer、訓練迴圈、Dropout | 必修 |
| M6 | [Attention引擎](module-m6-attention.html) | Tokenization／Embedding／Self-Attention／Multi-Head | 必修・核心 |
| M7 | [語言模型煉成](module-m7-llm-training.html) | GPT／BERT／T5、預訓練與微調、RLHF／DPO | 必修・核心 |
| M8 | [強化學習地圖](module-m8-reinforcement-learning.html) | MDP／Bellman／PPO（只求懂 RLHF 那一步） | 選修・查閱 |
| M9 | [專案還原室](module-m9-project-synthesis.html) | 用 M1～M8 的理論逐一還原 Threat Intel Agent 的技術決策 | 必修・收尾 |

## 設計原則

- 每個模組固定走「電梯簡報 → 底層概念（無案例）→ 逐層疊加 → 代入具體案例 → 類比鎖記憶 → 整體視覺總覽 → 業界實際應用案例 → 名詞卡 → 面試模擬 → 效率檢查點」十步版型（M3、M8 為選修略讀，走精簡版）。
- 地基永遠在案例前面：先建立跟任何應用都無關的最原始概念，疊加到完整機制後才代入具體案例，案例是拿來驗證理解，不是拿來替代理解。
- 每個模組收尾都有一題面試模擬問答，答案連回真實專案，目標是「答得出設計依据」而不是「背知識點」。
