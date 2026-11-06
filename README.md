# 【OKIYA式】MirrorRing ご利用説明書

制作正本 Ver.0.2に基づくWeb説明書です。
テレポートシステムの説明書に合わせ、白とピンクの配色、左側メニュー、クイックスタート優先の構成を採用しています。

## 構成

- index.html：本文・デザイン・ページ切替を含むWeb説明書
- .nojekyll：GitHub Pagesで静的ファイルをそのまま公開するための設定

外部ライブラリーやビルド処理は不要です。

## 公開方法

GitHubのSettings → Pagesで、SourceをDeploy from a branch、Branchをmain、フォルダーを/(root)に設定します。

## 画像を差し込む

index.html内のdata-shot属性で対応する枠を探します。
実画像をimagesフォルダーに追加し、該当するfigureの中身をimgとfigcaptionに置き換えます。
画像には説明文をalt属性として付け、style="max-width:100%;height:auto"を設定してください。
撮影画面と設定値を加工で変更せず、Inspectorの文字が読める画像を使用します。

- S01：MirrorRingを指に装着した状態 — SceneビューまたはVRChat実機画面。撮影環境を明記します。
- S02：UnityPackageのImport画面 — インポート対象が分かる実際の画面を掲載します。
- S03：Project内のMirrorRingのPrefab — 販売用UnityPackage内の保存場所が分かる画面を掲載します。
- S04：指ボーンとMirrorRingの親子関係 — HierarchyでMirrorRingが指ボーンの子になっている状態を掲載します。
- S05：Transformの調整 — InspectorのPosition・Rotation・Scaleが読める画面を掲載します。
- S06：指輪の装着位置 — Sceneビューで指輪の位置・向き・大きさを確認できる画面を掲載します。
- S07：Mirror Ringのラジアルメニュー — VRChat実機でON/OFFの操作箇所を撮影します。
- S08：ONとOFFの表示比較 — 同じ条件で撮影したVRChat実機のON画像とOFF画像を並べます。
- S09：RingMirrorマテリアルのInspector — Shader名とカメラ映像の設定項目が読める画面を掲載します。
- S10：Custom Imageの設定 — 画像の指定欄・Tiling・Offset・Blend・Tintを掲載します。
- S11：シルバー表現の設定 — Silver Colorと3つの明るさ設定を掲載します。
- S12：MatCapの設定 — Texture・Tiling・Offset・Strength・Tintを掲載します。

## 販売前の確認

- 依存パッケージ名と必要バージョンを確定し、はじめにへ反映する。
- 実画面のスクリーンショットを差し込む。
- UnityPackageの必要素材と参照切れを確認する。
- 新規プロジェクトでインポートを確認する。
- 同梱画像や素材の配布権利を確認する。
- 正本の確認済み動作と未確認事項を区別する。

公開済みのテレポートシステム説明書のファイルは変更していません。
