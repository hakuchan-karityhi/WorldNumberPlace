# World Sudoku — クレジット

本ドキュメントは、アプリ内「クレジット」から参照される第三者素材・オープンソースソフトウェアの帰属表示です。  
ライセンス全文は各配布元・同梱ファイルをご確認ください。

---

## 1. 本アプリケーション

**World Sudoku**（ワールドスドゥーク）のソフトウェア本体の著作権は、開発者（リポジトリ所有者）に帰属します。  
無断複製・改変・再配布を禁じます（ライセンス方針はリポジトリの `LICENSE` 等に従います）。

---

## 2. フォント（SIL Open Font License 1.1）

本アプリに同梱しているフォントは、いずれも **SIL Open Font License, Version 1.1** の下で提供されています。  
ライセンス全文は各フォントディレクトリ内の `OFL.txt`、および [SIL Open Font License 1.1](https://openfontlicense.org/open-font-license-official-text/) をご参照ください。

### Noto Sans JP（日本語 UI 用）

```
Copyright 2014-2021 Adobe (http://www.adobe.com/), with Reserved Font Name 'Source'

This Font Software is licensed under the SIL Open Font License, Version 1.1.
```

- 同梱パス: `world_sudoku/assets/font/Noto_Sans_JP/`
- ライセンス全文: `world_sudoku/assets/font/Noto_Sans_JP/OFL.txt`

### Noto Naskh Arabic（アラビア語 UI 用）

```
Copyright 2022 The Noto Project Authors (https://github.com/notofonts/arabic)

This Font Software is licensed under the SIL Open Font License, Version 1.1.
```

- 同梱パス: `world_sudoku/assets/font/Noto_Naskh_Arabic/`
- ライセンス全文: `world_sudoku/assets/font/Noto_Naskh_Arabic/OFL.txt`

### Noto Sans（欧文・汎用 UI 用）

```
Copyright 2022 The Noto Project Authors (https://github.com/notofonts/latin-greek-cyrillic)

This Font Software is licensed under the SIL Open Font License, Version 1.1.
```

- 同梱パス: `world_sudoku/assets/font/Noto_Sans/`
- ライセンス全文: `world_sudoku/assets/font/Noto_Sans/OFL.txt`

---

## 3. 数独パズル生成・求解ライブラリ（BSD 3-Clause）

### sudoku_dart

パズル生成および求解に [sudoku_dart](https://pub.dev/packages/sudoku_dart) を利用しています。

```
BSD 3-Clause License

Copyright (c) 2020, einsitang
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

- リポジトリ: <https://github.com/einsitang/sudoku-dart>

---

## 4. Flutter / Dart SDK

本アプリは [Flutter](https://flutter.dev/) および [Dart](https://dart.dev/) を用いて開発されています。  
SDK および付随ツールのライセンスは、Flutter の配布物に含まれるライセンス表示に従います（多くは BSD スタイルおよび各コンポーネントのライセンスの組み合わせ）。

---

## 5. 主要なオープンソースパッケージ（pub.dev）

以下は `world_sudoku/pubspec.yaml` に記載の **直接依存**を中心とした一覧です。  
正確な条文・著作権表示の一行は、各パッケージの `LICENSE` ファイルおよび [pub.dev](https://pub.dev/) の該当ページをご参照ください。  
（バージョンは `pubspec.lock` の解決結果に依存します。）

| パッケージ | 用途の概要 | ライセンス（pub.dev 上の表記） |
|-----------|------------|-------------------------------|
| `cupertino_icons` | iOS 風アイコン | MIT |
| `flutter_riverpod` / `riverpod_annotation` | 状態管理 | MIT |
| `flutter_localizations` / `intl` | 多言語・日付等 | BSD-3-Clause 等（SDK 由来を含む） |
| `shared_preferences` | ローカル永続化 | BSD-3-Clause |
| `go_router` | 画面遷移 | BSD-3-Clause |
| `url_launcher` | 外部ブラウザ起動 | BSD-3-Clause |
| `google_mobile_ads` | 広告表示 | Apache-2.0 |
| `in_app_purchase` | アプリ内課金 | BSD-3-Clause |
| `app_tracking_transparency` | iOS トラッキング許可 | MIT |
| `firebase_core` / `firebase_analytics` | Firebase 初期化・分析 | Apache-2.0 |

**開発時のみ（本番バイナリに含まれない場合があります）**

| パッケージ | 用途の概要 | ライセンス（一般的な表記） |
|-----------|------------|---------------------------|
| `build_runner` / `riverpod_generator` | コード生成 | BSD-3-Clause 等 |
| `flutter_lints` | 静的解析ルール | BSD-3-Clause |
| `flutter_launcher_icons` | アプリアイコン生成 | MIT |

上記以外にも、間接依存（transitive dependencies）として多数のパッケージが含まれます。  
完全な一覧・条文が必要な場合は、ビルド環境で `pubspec.lock` を基にしたライセンス収集ツールの利用を推奨します。

---

## 6. Google サービス（Firebase / AdMob）

本アプリは **Google Firebase**（例: Firebase Analytics）および **Google Mobile Ads（AdMob）** を利用する場合があります。  
これらの利用は、Google の各利用規約、ブランドガイドライン、およびプライバシーポリシーに準拠します。  
データの取り扱いは、アプリ内または配布物の **プライバシーポリシー** に記載のとおりです。

---

## 7. アプリ内画像アセット

盤面・数字パッド等で用いる **スクリプト別の数字画像**（`world_sudoku/assets/script_digits/` 配下）は、本プロジェクト用のアセットです。  
**作成には Anthropic 社の生成 AI「Claude」を使用しました。** 表示内容の選定・調整・組み込みは開発者が行っています。  
Unicode に基づく文字の見た目を表示するためのものであり、アプリにバンドルして配布しています。

---

## 8. アプリアイコン

ランチャー用の元画像 `world_sudoku/assets/images/app_icon.png` は、**Anthropic 社の生成 AI「Claude」を用いて作成しました。**  
各 OS 向けの解像度別アイコンは、`flutter_launcher_icons` によりこの画像から生成しています。

---

## 9. お問い合わせ

クレジット記載の修正・追加依頼は、アプリ内「お問い合わせ」からご連絡ください。

