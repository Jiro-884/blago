# Blago
[![License](https://img.shields.io/badge/License-CC--BY--1.0-green.svg)](https://github.com/Jiro-884/Blago\_flows/blob/main/LICENSE)
[![Coverage Status](https://coveralls.io/repos/github/Jiro-884/Blago/badge.svg?branch=Jiro-884-patch-1)](https://coveralls.io/github/Jiro-884/Blago?branch=Jiro-884-patch-1)
[![Rust Report Card](https://rust-reportcard.xuri.me/badge/github.com/jiro-884/blago)](https://rust-reportcard.xuri.me/report/github.com/jiro-884/blago)
[![DOI](https://zenodo.org/badge/784023239.svg)](https://zenodo.org/doi/10.5281/zenodo.12768586)


どんな形にも圧縮します
## Description
各種圧縮フォーマットを統一的なインタフェースで扱うもの

## アイコン
![logo](compress_tool.jpg)  

## Usage
```sh
blago [OPTIONS] <ARGUMENTS...>
OPTIONS
  -m, --mode <MODE>     操作モードを extract, archive, auto から選択する．デフォルトは auto.
  -d, --dest <DEST>     出力先のディレクトリを指定する．デフォルトは current directory.
  -o, --output <FILE>   アーカイブの出力ファイル．デフォルトは FlexPress.zip.
  -h, --help            helpメッセージを表示する．
ARGUMENTS
  extract mode: アーカイブファイルを展開する．
  archive mode: ファイルをアーカイブする.
  auto mode:    引数にアーカイブファイルが指定されている場合, 展開する.
                それ以外の場合, ファイルをアーカイブする．
 ```
 ## Install

```sh
brew install Jiro-884O/tap/blago
```

## Docker

```sh
docker run -it --rm -v $PWD:/workdir ghcr.io/jiro-884/blago:0.5.0 [OPTIONS] [ARGUMENTS]...
```

- **Working directory**: `/workdir`
- **User**: `nonroot`
