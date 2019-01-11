---
title: provisionedPlan リソースの種類
description: ユーザー エンティティと組織エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 7bed57761777e637fdc2e567d10aa7f741a86663
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837255"
---
# <a name="provisionedplan-resource-type"></a>provisionedPlan リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
  "@odata.type": "microsoft.graph.provisionedplan"
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
