# 保険詐欺検出モデル - Insurance Fraud Detection

本プロジェクトでは、保険請求データを用いて詐欺検出モデルを構築し、SHAP値による特徴量の可視化と解釈を行いました。  
実践的な不正検出を目的とし、精度・解釈性ともに高い分析を目指しました。  
*This project builds a fraud detection model using insurance claim data, incorporating SHAP-based feature interpretation to ensure both accuracy and explainability.*

---

## プロジェクト概要 / Project Overview

- **テーマ / Theme**：  
  保険請求データにおける詐欺検出  
  *Insurance fraud detection using claim data*

- **使用モデル / Models**：  
  決定木、ランダムフォレスト、XGBoost  
  *Decision Tree, Random Forest, XGBoost*

- **評価指標 / Evaluation Metrics**：  
  - F1スコア: `0.32` / *F1-score: `0.32`*  
  - ROC AUC: `0.86`  
  - PR AUC: `0.29` など / *and more*

- **注目特徴量 / Key Features**：  
  `Fault`, `BasePolicy`, `Days_Diff`, `Is_YoungDriver`

- **解釈手法 / Interpretability Method**：  
  SHAP（特徴量ごとの影響を可視化）  
  *SHAP (visualizing the impact of each feature)*

---

## 使用技術 / Tech Stack

| カテゴリ / Category     | 使用ライブラリ / Libraries            |
|------------------------|--------------------------------------|
| 言語 / Language         | Python                               |
| 分析 / Analysis         | Pandas, NumPy                        |
| モデル / Modeling       | scikit-learn, XGBoost                |
| 可視化 / Visualization  | Matplotlib, SHAP                     |
| 実行環境 / Environment  | Jupyter Notebook                     |

---

## モデル改善アプローチ / Model Optimization Approach

- **クラス不均衡への対応 / Class Imbalance Handling**：  
  SMOTE、`scale_pos_weight`、しきい値調整  
  *SMOTE, scale_pos_weight, threshold adjustment*

- **特徴量エンジニアリング / Feature Engineering**：  
  事故日と申請日の差分、若年ドライバー識別など  
  *Difference between accident and claim date, young driver flag, etc.*

- **評価軸の多角化 / Broadened Evaluation Metrics**：  
  AccuracyやF1に加え、PR AUCも重視  
  *Focus not only on accuracy and F1-score, but also on PR AUC*

- **解釈性の確保 / Ensuring Interpretability**：  
  SHAPによる特徴量の可視化・説明  
  *Feature importance analysis using SHAP*

---

## ファイル構成 / File Structure

```plaintext
insurance-fraud-detection/
├── insurance_fraud_detection_jp.ipynb   # 日本語ノートブック：前処理〜モデル構築・評価・可視化まで
│                                        # Notebook written in Japanese: preprocessing, modeling, evaluation, and SHAP visualization
├── insurance_fraud_detection_en.ipynb   # 英語ノートブック：内容は日本語版と同様、コメント・出力などすべて英語化
│                                        # Notebook written in English with the same content as JP version (fully translated comments & outputs)
└── README.md                            # 日本語＋英語の説明を併記したREADMEファイル
                                         # README file with both Japanese and English descriptions

---

## 今後の課題 / Future Work

- より高度なモデル（CatBoost, TabNetなど）の導入  
  *Implement more advanced models such as CatBoost and TabNet*

- 異常検知系手法（IsolationForest等）との比較  
  *Compare with anomaly detection methods like IsolationForest*

- ドメイン知識を活かした特徴量設計の追加  
  *Enhance feature engineering using domain-specific knowledge*

---

## お問い合わせ / Contact

- Author: Masahiro Okada  
- GitHub: [@MASAHIRO-700](https://github.com/MASAHIRO-700)
