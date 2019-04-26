---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の統計の概要。
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563435"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の役割の統計の概要。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedRoleSummary を取得する](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |privilegedRoleSummary オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevatedCount|int32|役割が割り当てられていて、役割がアクティブ化されているユーザーの数。|
|id|string| ロールの一意識別子。 読み取り専用。|
|managedcount|int32|役割が割り当てられているが、その役割が非アクティブ化されたユーザーの数。|
|mfaenabled|ブール値|役割のライセンス認証が MFA を必要とする場合は**true** 。 役割のライセンス認証が MFA を必要としない場合は**false** 。|
|status|string| 可能な値は、`ok`、`bad` です。 値は、の比率 (managedcount/ユーザーカウント) によって決まります。 比率が定義済みのしきい値よりも小さい`ok`場合は、が返されます。 それ以外`bad`の場合は、が返されます。|
|usersCount|int32|役割に割り当てられているユーザーの数。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
