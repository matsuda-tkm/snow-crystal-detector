# Snow Crystal Detector

## Google Colabでの実行方法

### 1. ノートブックを開く

https://colab.research.google.com/?hl=ja

### 2. GPU設定の確認

1. メニューから「ランタイム」→「ランタイムのタイプを変更」を選択
2. ハードウェアアクセラレータを「T4 GPU」に設定
3. 「保存」をクリック

### 3. リポジトリのクローン

```bash
!git clone https://github.com/matsuda-tkm/snow-crystal-detector.git
```

### 4. データセットの解凍

```bash
!unzip snow-crystal-detector/data/coco_dataset.zip
```


## ローカル環境での実行方法

### uvを使用する場合

```bash
git clone https://github.com/matsuda-tkm/snow-crystal-detector.git
cd snow-crystal-detector
uv sync
```

## ファイル構成

```
snow-crystal-detector/
├── notebooks/
│   ├── yolo.ipynb      # YOLO学習・推論ノートブック
│   └── rf.ipynb        # Random Forest実験ノートブック
├── data/
│   ├── dataset.zip     # Random Forest用データセット
│   └── coco_dataset.zip # YOLO形式データセット
├── coco.yaml           # データセット設定ファイル
├── pyproject.toml      # プロジェクト設定
└── README.md
```
