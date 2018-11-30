---
title: コネクタ リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072932"
---
# <a name="connector-resource-type"></a>コネクタ リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[コネクタを取得します。](../api/connector-get.md) | [コネクタ](connector.md) |コネクタ オブジェクトのプロパティと関係を参照してください。|
|[memberOf を一覧表示する](../api/connector-list-memberof.md) |[connectorGroup](connectorgroup.md)コレクション| コネクタに関連付けられている connectorGroup オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|externalIp|String|コネクタ コンピューターのサービスによって検出されたと外部の IP アドレスです。 読み取り専用|
|id|String| コネクタのオブジェクト id です。 <BR>読み取り専用。|
|マシン名|String| コネクタが実行されているマシンの名前です。 <BR>読み取り専用|
|status|文字列| コネクタの状態を示します。 使用可能な値は、`active`、`inactive` です。 読み取り専用 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|memberOf|[connectorGroup](connectorgroup.md)コレクション| 接続がのメンバーである connectorGroup。<br>読み取り専用。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
