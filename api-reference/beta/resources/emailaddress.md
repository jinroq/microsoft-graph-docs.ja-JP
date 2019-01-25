---
title: emailAddress リソースの種類
description: 名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc1f00ab09ac71f4f3cd9eb1aff8163a537ce257
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518668"
---
# <a name="emailaddress-resource-type"></a>emailAddress リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|address|String|エンティティ インスタンスの電子メール アドレスです。|
|name|String|エンティティ インスタンスの表示名。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/emailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
