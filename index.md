# ポートフォリオ
このページは、私が作成したAI・画像分類・3D作品などを紹介するポートフォリオです。

## プロジェクト一覧
- [犬猫画像分類モデル](https://github.com/suzuki2n/catdog288/tree/main)
- [業務効率化ツール]

## 現在作成中です

## Python業務効率化ツール
- 使用技術：Python, pandas, tkinter  
  実装内容：Excelファイルの読み込み → データ加工 → GUI操作でファイル出力  
- GitHub リンク：[○○○](https://github.com/suzuki2n/XXXX)

## ディープラーニング画像分類モデル（猫・犬）
- 犬猫分類AIモデル  
- 使用技術：TensorFlow, CNN, 転移学習（ResNet50 + Fine-tuning）  
- 精度：精度98.9%

このプロジェクトでは、転移学習とファインチューニングを使い、犬猫分類の精度を最大98.9%まで向上させました。  
モデルやコード、実験ログ（.ipynb）も全て公開中です。  
このリポジトリは、犬猫画像分類の転移学習プロジェクトの記録です。  
最終的に ResNet50＋Fine-tuning により **精度98.9%** を達成しました。

- このリポジトリに含まれるもの  
catdog_model_128.ipynb（CNNモデル）<br>
catdog_model_224.ipynb（CNNモデル）<br>
catdog_model_ResNet50_BATCH12_224.ipynb（実験中精度訳63％のモデル）<br>
catdog_model_ResNet50_BATCH16_224.ipynb（実験中精度訳63％のモデル）<br>
catdog_model_VGG16_BATCH8_224.ipynb（VGG16モデル精度93％）<br>
catdog_model_VGG16_BATCH16_224.ipynb（VGG16モデル精度93％）<br>

**完成モデル**  
catdog_model_ResNet50_BATCH16_FT2_224.ipynb（精度98.9％）<br>

img_resize.py（データセット用画像の前処理ツール）<br>
mkdir_learning.py（データセット用フォルダの作成ツール）<br>
perform_classification.py（モデルを実際の画像で実行、画像を分類保存するツール）<br>

順次プロジェクト内容を整理し、追加していきます。


