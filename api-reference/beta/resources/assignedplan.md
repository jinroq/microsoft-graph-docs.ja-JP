---
title: assignedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの両方の assignedPlans プロパティは、**assignedPlan** のコレクションです。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f699b635fb71d668cdd2a8fd11618786f3194d08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013270"
---
# <a name="assignedplan-resource-type"></a>assignedPlan リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ユーザー** エンティティと[組織](user.md)エンティティの両方の [assignedPlans](organization.md) プロパティは、**assignedPlan** のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|プランが割り当てられた日時です。例:2013-01-02T19:32:30Z。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|capabilityStatus|String|「有効」など。|
|service|String|サービスの名前。「Exchange」など。|
|servicePlanId|Guid|サービス プランを識別する GUID。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
