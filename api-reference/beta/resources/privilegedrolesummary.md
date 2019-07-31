---
title: privilegedRoleSummary リソースの種類
description: 特定の役割の統計の概要。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 30c9cfb93f8d20d30ad86d0f36019e87eae0ab65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965720"
---
# <a name="privilegedrolesummary-resource-type"></a>privilegedRoleSummary リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の役割の統計の概要。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedRoleSummary を取得する](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |PrivilegedRoleSummary オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|elevatedCount|int32|役割が割り当てられていて、役割がアクティブ化されているユーザーの数。|
|id|string| ロールの一意識別子。 読み取り専用です。|
|managedCount|int32|役割が割り当てられているが、その役割が非アクティブ化されたユーザーの数。|
|mfaEnabled|ブール値|役割のライセンス認証が MFA を必要とする場合は**true** 。 役割のライセンス認証が MFA を必要としない場合は**false** 。|
|status|string| 可能な値は、`ok`、`bad` です。 値は、の比率 (managedCount/ユーザーカウント) によって決まります。 比率が定義済みのしきい値よりも小さい`ok`場合は、が返されます。 それ以外`bad`の場合は、が返されます。|
|usersCount|int32|役割に割り当てられているユーザーの数。|

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
  "suppressions": []
}
-->
