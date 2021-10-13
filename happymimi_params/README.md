# happymimi_params
## Overview
happymimi_paramsは、ROSパラメータで使用するためのファイルを格納したパッケージです。<br>
このパッケージは以下を提供します。

- ロケーションデータをまとめたyamlファイル
- オブジェクトデータをまとめたyamlファイル

## Description

### ロケーションデータをまとめたyamlファイル
ロケーションに関するデータは[location]()ディレクトリに保存されます。<br>
このファイルは、ロケーションデータに関するパラメータである`/location_dict`として読み込まれます。

**location_dictの仕様**
| Key | Value |
|---|---|
| string型:`ロケーション名` | double:`座標(クォータニオン)` |

