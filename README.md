# 深層学習体験会 - Jupyter Notebook集

このリポジトリは、深層学習の様々な技術を実際に体験できるJupyter Notebookのコレクションです。

## 🎯 このリポジトリについて

最新のAI技術（画像生成、動画生成、音声合成、LLMなど）を、Google Colabで無料で体験できます。プログラミング初心者でも、セルを順番に実行するだけで動作するように設計されています。

## 📋 必要な環境

- **Google Colab**（推奨）
  - 無料のT4 GPUで実行可能
  - ブラウザだけで動作
  - 環境構築不要
- **Google Drive**（画像保存用）

## 🚀 使い方

1. 下記の「Open in Colab」バッジをクリック
2. Google Colabで開いたら、上部メニューから「ランタイム」→「すべて実行」を選択
3. 各セルのマークダウン解説を読みながら実行結果を確認

## 📚 Notebook一覧

### 🖼️ 画像処理系（CPU対応）

#### 01. 深度推定（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/01_深度推定_CPU.ipynb)

**技術**: Depth-Anything-V2-Small
**内容**: 1枚の画像から奥行き情報を推定
**応用例**: 自動運転、3D復元、ARアプリ
**実行時間**: 約2-3分

---

#### 02. 画像分類（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/02_画像分類_CPU.ipynb)

**技術**: Vision Transformer (ViT)
**内容**: NSFW画像検出モデルで画像の適切性を判定
**応用例**: コンテンツモデレーション、フィルタリング
**実行時間**: 約1-2分
**推奨**: 最もシンプルで初心者向け

---

#### 03. バーコード検出（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/03_バーコード検出_CPU.ipynb)

**技術**: YOLOv8
**内容**: 画像内のバーコードを自動検出
**応用例**: 在庫管理、自動レジ、物流
**実行時間**: 約2-3分

---

#### 04. 背景除去（CPU）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/04_背景除去_CPU.ipynb)

**技術**: RMBG-1.4
**内容**: 画像から前景と背景を分離し、背景を透明化
**応用例**: ECサイト商品画像、バーチャル背景、写真編集
**実行時間**: 約2-3分

---

### 🎬 動画生成系（T4 GPU推奨）

#### 05. 画像間動画生成（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/05_画像間動画生成_T4.ipynb)

**技術**: LTX-Video
**内容**: 2枚の画像から滑らかな動画を生成
**応用例**: アニメーション制作、商品プレゼンテーション
**実行時間**: 約10-15分
**注意**: シンプルな遷移に適しています（激しい動きには不向き）

---

#### 06. テキスト動画生成（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/06_テキスト動画生成_T4.ipynb)

**技術**: LTX-Video
**内容**: テキストプロンプトだけから動画を生成
**応用例**: 絵コンテ作成、広告動画、ストーリーボード
**実行時間**: 約10-20分
**ヒント**: 詳細なプロンプトを書くと良い結果が得られます

---

### 🎨 画像編集系（T4 GPU推奨）

#### 07. AI画像編集（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/07_AI画像編集_T4.ipynb)

**技術**: Instruct-Pix2Pix (Stable Diffusion)
**内容**: テキスト指示で画像を編集
**応用例**: 写真のスタイル変更、オブジェクト追加、色調補正
**実行時間**: 約5-10分
**編集例**:
- "turn him into cyborg"（サイボーグに変える）
- "make the background dark and ominous"（背景を暗く不気味に）
- "add sunglasses"（サングラスを追加）

---

### 🎤 音声生成系

#### 08. 音声合成（TTS）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/08_音声合成_TTS_T4.ipynb)

**技術**: Zonos TTS
**内容**: テキストから音声を生成（多言語対応、感情表現可能）
**応用例**: オーディオブック、ナレーション、アクセシビリティ
**実行時間**: 約5-10分（初回モデルロード含む）
**特徴**:
- 約100言語対応（日本語含む）
- 感情パラメータ調整可能
- 声のクローニング機能

---

### 🤖 大規模言語モデル系（T4 GPU推奨）

#### 09. LLMファインチューニング（T4）
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yukimaru77/beginner-deep-learning-/blob/main/09_LLMファインチューニング_T4.ipynb)

**技術**: Llama 3.1 8B + Unsloth + LoRA
**内容**: 大規模言語モデルのファインチューニング
**応用例**: カスタムチャットボット、ドメイン特化型AI
**実行時間**: 約10-30分（60ステップ）
**学べること**:
- LoRA（効率的な学習手法）
- データセットの準備
- モデルの保存と読み込み

---

## 💡 各技術の難易度

| Notebook | 難易度 | GPU要件 | 実行時間 |
|---------|--------|---------|---------|
| 01. 深度推定 | ⭐☆☆☆☆ | CPU可 | 2-3分 |
| 02. 画像分類 | ⭐☆☆☆☆ | CPU可 | 1-2分 |
| 03. バーコード検出 | ⭐☆☆☆☆ | CPU可 | 2-3分 |
| 04. 背景除去 | ⭐☆☆☆☆ | CPU可 | 2-3分 |
| 05. 画像間動画生成 | ⭐⭐⭐☆☆ | T4推奨 | 10-15分 |
| 06. テキスト動画生成 | ⭐⭐⭐☆☆ | T4推奨 | 10-20分 |
| 07. AI画像編集 | ⭐⭐☆☆☆ | T4推奨 | 5-10分 |
| 08. 音声合成 | ⭐⭐☆☆☆ | CPU可 | 5-10分 |
| 09. LLMファインチューニング | ⭐⭐⭐⭐☆ | T4推奨 | 10-30分 |

## 🎓 推奨される学習順序

### 初心者向けコース
1. **02. 画像分類** - 最もシンプル
2. **01. 深度推定** - 画像処理の基礎
3. **04. 背景除去** - 実用的な技術

### 中級者向けコース
4. **03. バーコード検出** - 物体検出の入門
5. **07. AI画像編集** - プロンプトエンジニアリング
6. **08. 音声合成** - パラメータ調整を体験

### 上級者向けコース
7. **05. 画像間動画生成** - 動画生成の基礎
8. **06. テキスト動画生成** - 高度な動画生成
9. **09. LLMファインチューニング** - 最も高度な技術

## 📝 よくある質問

### Q: Google Colabで「GPUなし」と表示されます
**A**: 「ランタイム」→「ランタイムのタイプを変更」→「T4 GPU」を選択してください。

### Q: メモリ不足エラーが出ます
**A**:
- 「ランタイム」→「ランタイムを出荷時設定にリセット」を試してください
- 動画生成の場合、フレーム数や解像度を下げてください

### Q: どのNotebookから始めればいいですか？
**A**: **02. 画像分類**が最もシンプルで、2分程度で完了します。

### Q: 自分の画像を使いたい
**A**: Google Driveを接続し、`/MyDrive/images/`フォルダに画像をアップロードしてください。

### Q: エラーが出たらどうすればいいですか？
**A**:
1. ランタイムをリセット
2. 最初からすべて実行
3. それでも解決しない場合は、エラーメッセージを確認

## 🔧 トラブルシューティング

### インストールエラー
```bash
# セルを再実行するか、ランタイムをリセット
```

### GPUメモリ不足
- バッチサイズを減らす
- 解像度を下げる
- フレーム数を減らす

### モデルダウンロードの失敗
- インターネット接続を確認
- セルを再実行

## 📚 参考リンク

- [Hugging Face](https://huggingface.co/) - モデルのソース
- [Google Colab](https://colab.research.google.com/) - 実行環境
- [Unsloth](https://unsloth.ai/) - LLMファインチューニング

## 🤝 体験会での注意事項

1. **時間配分**: 各Notebookの実行時間を考慮してください
2. **順番**: 簡単なものから試すことをお勧めします
3. **保存**: 結果はGoogle Driveに保存されます
4. **質問**: 分からないことがあれば、マークダウンセルの解説を参照してください

## 📄 ライセンス

各モデルには独自のライセンスがあります。商用利用の際は各モデルのライセンスを確認してください。

---

**作成日**: 2025年10月
**対象**: 深層学習体験会参加者
**環境**: Google Colab（無料版で動作確認済み）
