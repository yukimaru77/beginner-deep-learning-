# 深層学習体験 - Jupyter Notebook集

このリポジトリは、深層学習の様々な技術を実際に体験できるJupyter Notebook(Pythonで書かれたプログラム)のコレクションです。

## 🎯 このリポジトリについて

最新のAI技術（画像生成、動画生成、音声合成、LLMなど）を、Google Colabというサービスを使ってで無料で動かせます。セルを順番に実行するだけで動作するように設計してます。

## 📋 必要なもの

- PC
- Google アカウント(gmailとかを使っているなら持っています)

## 🚀 使い方

1. 下記の「Open in Colab」バッジをクリック
2. 上から順番にセルを実行

## 📚 Notebook一覧

### 🖼️ 画像処理系（CPU対応）

#### 01. 深度推定（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/01_深度推定_CPU.ipynb)

**技術**: Depth-Anything-V2-Small
**内容**: 1枚の画像から奥行き情報を推定
**応用例**: 自動運転、3D復元、ARアプリ

---

#### 02. 画像分類（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/02_画像分類_CPU.ipynb)

**技術**: Vision Transformer (ViT)
**内容**: NSFW画像検出モデルで画像の適切性を判定
**応用例**: SNSやGoogle画像検索のフィルタリング

---

#### 03. バーコード検出（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/03_バーコード検出_CPU.ipynb)

**技術**: YOLOv8
**内容**: 画像内のバーコードを自動検出
**応用例**: 在庫管理、自動レジ、物流

---

#### 04. 背景除去（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/04_背景除去_CPU.ipynb)

**技術**: RMBG-1.4
**内容**: 画像から前景と背景を分離し、背景を透明化
**応用例**: ECサイト商品画像、バーチャル背景、写真編集

---

### 🎬 動画生成系（T4 GPU推奨）

#### 05. 画像間動画生成（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/05_画像間動画生成_T4.ipynb)

**技術**: LTX-Video
**内容**: 2枚の画像から滑らかな動画を生成

---

#### 06. テキスト動画生成（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/06_テキスト動画生成_T4.ipynb)

**技術**: LTX-Video
**内容**: テキストプロンプトだけから動画を生成

---

### 🎨 画像編集系（T4 GPU推奨）

#### 07. AI画像編集（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/07_AI画像編集_T4.ipynb)

**技術**: Instruct-Pix2Pix (Stable Diffusion)
**内容**: テキスト指示で画像を編集

---

### 🎤 音声生成系

#### 08. 音声合成（TTS）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/08_音声合成_TTS_T4.ipynb)

**技術**: Zonos TTS
**内容**: テキストから音声を生成（多言語対応、感情表現可能）

---

### 🤖 大規模言語モデル系（T4 GPU推奨）

#### 09. LLMファインチューニング（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/09_LLMファインチューニング_T4.ipynb)

**技術**: Llama 3.1 8B + Unsloth + LoRA
**内容**: 大規模言語モデルのファインチューニング
**学べること**:
- LoRA（効率的な学習手法）
- データセットの準備
- モデルの保存と読み込み
