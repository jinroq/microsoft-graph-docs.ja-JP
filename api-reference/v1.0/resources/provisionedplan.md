---
title: provisionedPlan リソースの種類
description: ユーザー エンティティと組織エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: dd8d4f5b406a2291a829d7c11d4948bd9a08d453
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831487"
---
# <a name="provisionedplan-resource-type"></a>provisionedPlan リソースの種類

[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|capabilityStatus|String|「有効」など。|
|provisioningStatus|String|「成功」など。|
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
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
