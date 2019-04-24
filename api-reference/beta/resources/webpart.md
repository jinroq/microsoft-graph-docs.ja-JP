---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453610"
---
# <a name="webpart-resource"></a>webPart リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**webPart**リソースは、[サイトページ](sitepage.md)上の web パーツの種類とレンダリング情報を表します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>プロパティ

| プロパティ                | 型             | 説明
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | webPart の種類を指定する一意の識別子。 値の取得のみ可能です。
| **data**                | [sitepagedata][] | webpart に必要なプロパティ (webpart によって異なります)

[sitepagedata]: sitepagedata.md

## <a name="remarks"></a>解説

Web パーツでは、**データ**の下に必要なプロパティを定義できます。

ページの詳細については、「 [sitepage](sitepage.md)」を参照してください。
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
