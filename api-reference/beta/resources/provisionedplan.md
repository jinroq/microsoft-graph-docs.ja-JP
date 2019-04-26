---
title: provisionedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの provisionedPlans プロパティは、**provisionedPlan** のコレクションです。'
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563348"
---
# <a name="provisionedplan-resource-type"></a>provisionedPlan リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ユーザー** エンティティと[組織](user.md)エンティティの [provisionedPlans](organization.md) プロパティは、**provisionedPlan** のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|capabilityStatus|String|「有効」など。|
|プロビジョニング状態|String|「成功」など。|
|service|String|サービスの名前。「AccessControlS2S」など。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
