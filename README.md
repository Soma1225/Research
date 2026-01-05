# Research

## Project Structure

```
Research/
├── notebooks/     # Jupyter notebooks (Colab対応)
├── src/           # ソースコード
├── data/          # データファイル (git管理外)
├── requirements.txt
└── README.md
```

## Google Colabでの実行方法

### 1. リポジトリをクローン

ノートブックの最初のセルで以下を実行:

```python
!git clone https://github.com/YOUR_USERNAME/Research.git
%cd Research
```

### 2. 依存関係をインストール

```python
!pip install -r requirements.txt
```

### 3. srcをインポートパスに追加

```python
import sys
sys.path.append('/content/Research')

# これで src/ 内のモジュールをインポートできる
# from src import your_module
```

## ローカル環境での実行

```bash
# リポジトリをクローン
git clone https://github.com/YOUR_USERNAME/Research.git
cd Research

# 仮想環境を作成 (推奨)
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# 依存関係をインストール
pip install -r requirements.txt

# Jupyter Notebookを起動
jupyter notebook
```

## 開発

- `notebooks/`: 実験・分析用のJupyter notebooks
- `src/`: 再利用可能なPythonモジュール
