# happymimi_msgs
## Overview
使用頻度の高いROSメッセージやサービスファイルが置かれたパッケージです。

# Description

### メッセージファイルたち

- ### [SerInt.msg](./msg/StrInt.msg)
> stfing型、int8型のメッセージ

| Message |
|---|
| string型: `data`、int8型: `num` |


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
