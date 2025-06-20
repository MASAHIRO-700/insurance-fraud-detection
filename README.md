# 保険詐欺検出モデル - Insurance Fraud Detection

本プロジェクトは、保険請求データを用いて詐欺検出モデルを構築し、SHAP値を用いた特徴量の可視化と解釈を行ったものです。  
機械学習による実用的な不正検出を目的とし、精度・解釈性ともに高い分析を目指しました。

---

## 📌 プロジェクト概要

- 🔍 **テーマ**：保険請求データにおける詐欺検出
- 🧠 **使用モデル**：単純な決定木、ランダムフォレスト、XGBoost
- 📊 **評価指標**：  
  - F1-score：0.61  
  - ROC AUC：0.96
- 💡 **注目特徴量**：Fault, BasePolicy（SHAPにより影響が大きいことが判明）
- 🛠️ **使用ツール・ライブラリ**：Python, Pandas, scikit-learn, SHAP, Jupyter Notebook

---

## 📁 ファイル構成

| ファイル名 | 内容 |
|------------|------|
| `fraud_detection_shap.ipynb` | 詐欺検出モデルの構築とSHAPによる分析を行ったNotebook |
| `fraud_detection_summary.pdf`（任意） | NotebookをPDFに変換した要約版（職務経歴書に添付する場合など） |

---

## 👤 作成者

- 氏名：MASAHIRO-700
- GitHub：https://github.com/MASAHIRO-700
- 分析・データサイエンスに関心がある方は、ぜひご覧ください
