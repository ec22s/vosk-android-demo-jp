# vosk-android-demo-jp

音声認識ライブラリ VOSK の Android 用公式デモで日本語を使うテスト（2026年2月）

<br>

## 参考URL

- フォーク元 https://github.com/alphacep/vosk-android-demo

- VOSK トップ https://alphacephei.com/vosk/

- 日本語記事「【Kotlin】Androidで連続して音声認識がしたい」

  https://dev.classmethod.jp/articles/kotlin-android-vosk/

<br>

## 概要

- 修正点

  - Javaを21に、gradleを9.0に上げた

  - ソース中の言語モデルのパスを日本語用に変更

  - 言語モデル本体をリポジトリから除外（ファイルサイズ大きいため）

- ビルド確認環境（2026年2月）

    ```
    Android Studio Panda 1 | 2025.3.1 Patch 1
    Build #AI-253.29346.138.2531.14876573, built on February 12, 2026
    Runtime version: 21.0.9+-14649483-b1163.86 x86_64
    VM: OpenJDK 64-Bit Server VM by JetBrains s.r.o.
    Toolkit: sun.lwawt.macosx.LWCToolkit
    macOS 26.3
    GC: G1 Young Generation, G1 Concurrent GC, G1 Old Generation
    Memory: 2048M
    Cores: 20
    Metal Rendering is ON
    Registry:
    ide.experimental.ui=true
    ```

- 動作確認端末（2026年2月）

  - BPad Mini SE (Android 15)

<br>

## 使用手順

- リポジトリをダウンロード

- 言語モデルのページ https://alphacephei.com/vosk/models

  → Japanese → vosk-model-small-ja-0.22 をダウンロード

- ダウンロードしたZIPを解凍

- ディレクトリ名 `vosk-model-small-ja-0.22` を `model-small-ja-0.22` に変更（長いので）、`models/src/main/assets/` に置く

- 実行環境を確認（Javaが21である等）、ビルド


<br>

## 付記

- 1GBある大規模日本語モデルは試していません

- 質問等あれば[プロフィール](https://github.com/ec22s)のEメールへご連絡下さい

- 以下フォーク元のREADMEです

<br>

## About

This demo implements offline speech recognition and speaker identification for mobile applications using Kaldi and Vosk libraries.

Check the [releases](https://github.com/alphacep/vosk-android-demo/releases) for pre-built binaries.

## Documentation

For documentation and instructions please visit the [Vosk Website](https://alphacephei.com/vosk/android).
