# npa-rta

[警察庁:交通事故統計情報のオープンデータ](https://www.npa.go.jp/publications/statistics/koutsuu/opendata/index_opendata.html) の 2019 ～ 2022 の CSV データを累積的に Mapbox Vector Tile 形式に変換したデータセットです。

# タイル仕様

| URL          | <https://indigo-lab.github.io/npa-rta/{z}/{x}/{y}.pbf> |
| ------------ | ------------------------------------------------------ |
| データソース | 警察庁オープンデータ：交通事故統計情報 2019-2022,本票  |
| ズームレベル | 14                                                     |
| 作成日時     | 2024 年 3 月 28 日                                     |

## レイヤー定義

以下のレイヤーを含んでいます。

| source-layer | description                             |
| ------------ | --------------------------------------- |
| accident     | 交通事故情報 (Point) を収納したレイヤー |

## ID 情報

「公表年」「都道府県コード」「警察署等コード」「本票番号」を連結して数値としてパースしたものを GeoJSON Feature の id として採用しています。

## seeAlso

- <https://github.com/indigo-lab/npa-rta-2019>
