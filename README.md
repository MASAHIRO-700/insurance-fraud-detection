# 保険詐欺検出モデル - Insurance Fraud Detection

本プロジェクトでは、保険請求データを用いて詐欺検出モデルを構築し、SHAP値による特徴量の可視化と解釈を行いました。  
実践的な不正検出を目的とし、精度・解釈性ともに高い分析を目指しました。

---

## Project Overview

This project aims to build a machine learning model that detects insurance fraud using structured claim data.  
It includes not only model training and evaluation but also interpretability analysis with SHAP.

---

## プロジェクト概要 / Project Summary

-  **テーマ / Theme**: 保険請求データにおける詐欺検出 / Insurance Fraud Detection
-  **使用モデル / Models**: 決定木、ランダムフォレスト、XGBoost
-  **評価指標 / Metrics**:
  - F1-score: `0.32`
  - ROC AUC: `0.86`
  - PR AUC: `0.29` など
-  **注目特徴量 / Key Features**: `Fault`, `BasePolicy`, `Days_Diff`, `Is_YoungDriver`
-  **解釈手法 / Interpretability**: SHAP（特徴量ごとの影響を可視化）

---

## 使用技術 / Tech Stack

| カテゴリ | 使用ライブラリ |
|----------|----------------|
| 言語 / Language | Python |
| 分析 / Analysis | Pandas, NumPy |
| モデル / Modeling | scikit-learn, XGBoost |
| 可視化 / Visualization | Matplotlib, SHAP |
| 実行環境 / Environment | Jupyter Notebook |

---

## モデル改善アプローチ / Model Optimization

-  **クラス不均衡への対応**：SMOTE, `scale_pos_weight`, しきい値調整
-  **特徴量エンジニアリング**：事故日と申請日の差分、年齢に基づく若年ドライバー識別
-  **評価軸の多角化**：Accuracy/F1だけでなく、PR AUCにも注目
-  **SHAPによる特徴量重要度の可視化と解釈**

---

## ファイル構成 / File Structure
insurance-fraud-detection/
├── fraud_detection_shap.ipynb # メインノートブック（モデル構築〜可視化まで）
└── README.md # 本ファイル

---

## 今後の課題 / Future Work

- より高度なモデル（CatBoost, TabNetなど）の導入
- 異常検知系手法（IsolationForest等）との比較
- ドメイン知識を活かした特徴量設計の追加

---

## お問い合わせ / Contact

- Author: Masahiro Okada  
- GitHub: [@MASAHIRO-700](https://github.com/MASAHIRO-700)
