---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640176"
---
# <a name="webpart-resource"></a>web パーツ リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Web パーツ**リソースは、型との[sitePage](sitepage.md)上の web パーツのレンダリング情報を表します。

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
| **type**                | String           | Web パーツの種類を指定する一意の識別子です。 読み取り専用です。
| **data**                | [sitePageData][] | Web パーツ (web パーツによって異なります) に必要なプロパティ

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>注釈

Web パーツは、[**データ**の独自の必要なプロパティを定義できます。

ページの詳細については、 [sitePage](sitepage.md)を参照してください。
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
