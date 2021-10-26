# happymimi_msgs
## Overview
使用頻度の高いROSメッセージやサービスファイルが置かれたパッケージです。

# Description

### メッセージファイルたち

- ### [SerInt.msg](./msg/StrInt.msg)
> リクエストなしの、レスポンスがstring型のサービス

| Message |
|---|
| string型: `data`<br>int8: `num` |


### サービスファイルたち

- ### [SetStr.srv](./srv/SetStr.srv)
> リクエストなしの、レスポンスがstring型のサービス

| Request | Result |
|---|---|
| None | string型: `result` |

- ### [SimpleTrg.srv](./srv/SimpleTrg.srv)
> リクエストなしの、レスポンスがbool型のサービス

| Request | Result |
|---|---|
| None | bool型: `result` |

- ### [StrTrg.srv](./srv/StrTrg.srv)
> リクエストがstring型で、レスポンスがbool型のサービス

| Request | Result |
|---|---|
| string型: `data` | bool型: `result` |

# Usage
アーメン
