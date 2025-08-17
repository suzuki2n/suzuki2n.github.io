# ポートフォリオ
このページは、私が作成したAI・画像分類・3D作品などを紹介するポートフォリオです。<br>
私は独学でプログラミングを学習しています。Python開発とツール作成において、ChatGPT、Claude、Geminiなどの生成AIを積極的に活用しています。<br><br>

# 開発アプローチ
- 企画段階：各AIと相談しながら「何を作成したいか」を明確化
- 実装段階：AIにコード生成を依頼後、自分でコード内容を確認・理解
- 改善段階：目的通りの動作になるまで試行錯誤を重ね、完成度を高める

# 具体的な活用事例
- 犬猫分類プロジェクトでは、ResNet50転移学習モデルで期待した精度が得られなかった際、3つのAI（ChatGPT・Claude・Gemini）の力を借りて原因分析を行い、最終的に問題を解決して完成させました。
- 猫の切り抜きツールでは、主にChatGPTを使用してコード作成を進め、不明な点についてはClaudeから詳細な解説やアドバイスを受けて理解を深めました。

## プロジェクト一覧
- [犬猫画像分類モデル](https://github.com/suzuki2n/catdog288/tree/main)
- [猫の自動切り抜き]

## 現在作成中です

## ディープラーニング画像分類モデル（猫・犬）
- 犬猫分類AIモデル  
- 使用技術：TensorFlow, CNN, 転移学習（ResNet50 + Fine-tuning）  
- 精度：精度98.9%

このプロジェクトでは、転移学習とファインチューニングを使い、犬猫分類の精度を最大98.9%まで向上させました。<br>  
モデルやコード、実験ログ（.ipynb）も全て公開中です。<br>  
このリポジトリは、犬猫画像分類の転移学習プロジェクトの記録です。<br>  
最終的に ResNet50＋Fine-tuning により **精度98.9%** を達成しました。<br>

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


## 猫の自動切り抜き（YOLOv8-seq + OpenCV）
### 概要
- 目標：大量の画像から猫だけを抽出し、透過PNGを自動生成
- 学習目的：YOLOの実装手順とDockerの使い方を習得
- 技術：Ultralytics YOLOv8-seg（推論のみ / 学習なし）＋ OpenCV。
- システム構成：前処理→推論→切り抜き→QCの完全バッチ処理
- 開発環境：Docker、ubuntu
- 品質管理：仕上がり判定のためのQCツールを実装

### 学習内容
- WSL2 + Docker + GPU での環境構築・運用
- VS Code の Dev Containers でコンテナ内での開発・実行
- 画像前処理（縮小/拡大、CLAHE、軽いシャープ）

### 手順
- 1. preprocess.py：小さい画像を拡大、低コントラストを CLAHE で補正
- 2. cutout_batch.py：YOLOv8-seg 推論 → マスク合成 → 透過 PNG 保存（穴が大きい/マスク無は GrabCut 保険）
- 3. qc_cutouts.py：面積・端接触・穴・連結成分で ok / review を自動仕分け









順次プロジェクト内容を整理し、追加していきます。<br>


## 3Dモデル・作品紹介
### 3D小道具：琴<br>
フォーマット：FBX形式<br>
使用シェーダー：Standard<br>
無料配布中（Booth）<br>
▶ [配布ページはこちら](https://suzuki2n.booth.pm/items/3971677)
はこちら<br>

### VRMアバター<br>
VRoid Hubにて公開中<br>
▶ [VRMモデルを見る](https://hub.vroid.com/characters/6889964990498381032/models/4232243861661725226)
<br>

