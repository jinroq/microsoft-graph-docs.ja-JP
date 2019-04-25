---
title: コネクタリソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535537"
---
# <a name="connector-resource-type"></a>コネクタリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[コネクタの取得](../api/connector-get.md) | [コネクター](connector.md) |コネクタオブジェクトのプロパティとリレーションシップを読み取ります。|
|[List memberOf](../api/connector-list-memberof.md) |[コネクタグループ](connectorgroup.md)コレクション| コネクタに関連付けられているコネクタグループオブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|externalip|String|コネクタコンピューターのサービスによって検出された外部 IP アドレス。 読み取り専用|
|id|String| コネクタのオブジェクト id。 <BR>読み取り専用。|
|マシン|String| コネクタが実行されているコンピューターの名前。 <BR>読み取り専用|
|status|string| コネクタの状態を示します。 可能な値は、`active`、`inactive` です。 読み取り専用 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|memberOf|[コネクタグループ](connectorgroup.md)コレクション| 接続がメンバーであるコネクタグループ。<br>読み取り専用。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
