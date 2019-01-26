---
title: insightIdentity
description: 共有アイテムのプロパティを格納する複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 47283a82260d4f03a271a16660d58aca60da94e1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577229"
---
# <a name="insightidentity"></a>insightIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[共有](insights-shared.md)アイテムのプロパティを格納する複合型。 

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |-----------    | -------------|
| displayName       | String          | アイテムを共有するユーザーの表示名。 |
| id              | String        | アイテムを共有するユーザーの id です。     |
| address             | String      | アイテムを共有するユーザーの電子メール アドレスです。  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
