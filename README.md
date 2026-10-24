# Kotobagraph（コトバグラフ）

音声・動画ファイルから、日本語の文字起こしを作る Windows 用の無料アプリです。
OpenAI の音声認識モデル Whisper を使い、すべてお使いのパソコンの中で処理します（音声データは外部に送信されません）。

*A free Windows app that transcribes audio and video files into text, entirely on your own PC, using Whisper models. (Japanese UI only.)*

## できること

- **ファイルをドロップするだけ**：音声・動画ファイルをウィンドウに入れると、文字起こしを始めます
- **モデルを選べる**：迷ったときの `large-v3-turbo`、日本語特化の `kotoba-whisper-v2.0`、最高精度の `large-v3`、軽い `small`
- **GPU で速くなる**：NVIDIA（CUDA）に加え、AMD / Intel の GPU（Vulkan）にも対応。GPU が無くても CPU で動きます
- **自動品質チェック**：自信の低い所や同じ言葉の繰り返しだけを、自動で聞き直します
- **リアルタイム議事録**（v1.5.0〜）：マイクの声をその場で文字起こしし、決定事項・アクション・保留事項などを含む議事録を自動で作ります（AI もパソコンの中で動き、外部に送信されません）。録音は MP3 で保存
- **AI・議事録への連携**：フィラー（「えー」など）を取り除いた文章や、議事録用の指示文付きの文章を、ワンクリックでコピー
- テキストファイルは、音声ファイルと同じ場所に自動で保存されます

## ダウンロードと使い方

1. [Releases](https://github.com/retzrs-ops/Kotobagraph-release/releases/latest) から、最新の **`Kotobagraph_v〇〇.zip`** をダウンロードします。
2. zip を右クリック →「すべて展開」。展開したフォルダの `Kotobagraph.exe` を起動します。
   - 青い警告「WindowsによってPCが保護されました」が出たら、「詳細情報」→「実行」を押してください（電子署名が付いていないための警告です）。
3. くわしい使い方は、**[説明書](https://retzrs-ops.github.io/Kotobagraph-release/)** をご覧ください。

## 動作環境

- Windows 10 / 11（64bit）
- インターネット接続（初回のモデル、FFmpeg、議事録用 AI のダウンロードに使います。そのあとは、ネットが無くても文字起こしできます）
- 空き容量：使うモデルに応じて、約 1〜4 GB（リアルタイム議事録の AI を使うときは、さらに約 2.5 GB）
- マイク（リアルタイム議事録を使うとき）

## ライセンス・免責

- 利用条件は [LICENSE](LICENSE)、同梱している第三者ソフトウェアのライセンスは [THIRD_PARTY_LICENSES.txt](THIRD_PARTY_LICENSES.txt) をご覧ください。
- 文字起こしの結果には誤りが含まれることがあります。大切な用途では、必ずご自身で確認してください。
- ソースコードは公開していません。

(c) 2026 Retzn
