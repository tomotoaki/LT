# LT教材リポジトリ

## 概要

このリポジトリは、ライトニングトーク（LT）用の教材を管理するためのものです。
教材は、`prompt`の指示書に基づいて、Marp for VS Code形式で作成されています。

## ディレクトリ構成

```
.
├── prompt/            # 生成AIへの指示書
├── images/            # Markdownファイル内で使用する画像ファイル
├── pdf/               # Marp for VS CodeからエクスポートされたPDFファイル
├── pptx/              # Marp for VS CodeからエクスポートされたPowerPointファイル
├── *.md               # Marp for VS Code形式のMarkdownソースファイル (ルート直下)
└── README.md          # このファイル
```

## 資料の作成とエクスポート手順

1.  **資料作成**:
    * `prompt`に教材のテーマに即した指示書を作成します。
    * 指示書を元に、生成AIを利用してMarp for VS Code形式のMarkdownファイルを生成します。
    * スライド内で使用する画像は `images/` ディレクトリに配置し、Markdownファイル内から相対パスで参照します。
        例: `![bg right:40%](images/flow.png)`

2.  **エクスポート**:
    *   VS Codeで編集したMarkdownファイルを開きます。
    *   Marp for VS Code拡張機能の機能を利用して、資料をHTML形式またはPDF形式にエクスポートします。
        *   コマンドパレット (Ctrl+Shift+P or Cmd+Shift+P) から `Marp: Export slide deck...` を選択します。
        *   エクスポート形式を選択します。
    *   エクスポートされたファイルは、それぞれ対応するディレクトリに格納します。
        *   PDFファイル: `pdf/` ディレクトリ
        *   PowerPointファイル: `pptx/` ディレクトリ

## 使用ツール

*   Marp for VS Code: Markdownからスライドを作成するためのVS Code拡張機能。
