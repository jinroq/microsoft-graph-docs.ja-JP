---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の概要統計情報です。
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513740"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の役割の概要統計情報です。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleSummary を取得します。](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |PrivilegedRoleSummary オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevatedCount|int32|割り当てられているロールおよびロールを持つユーザーの数がアクティブになります。|
|id|string| ロールの一意の識別子です。 読み取り専用です。|
|managedCount|int32|役割が割り当てられているユーザーが、ロールの数が無効になります。|
|mfaEnabled|boolean|**真**の役割のアクティブ化には、MFA が必要な場合です。 **false**の役割のアクティブ化は、MFA を必要としない場合。|
|status|string| 使用可能な値は、`ok`、`bad` です。 値の比率によって異なります (managedCount/usersCount)。 割合は、定義済みのしきい値より小さい場合は、`ok`が返されます。 それ以外の場合、`bad`が返されます。|
|usersCount|int32|ロールに割り当てられているユーザーの数です。|

## <a name="relationships"></a>リレーションシップ
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
