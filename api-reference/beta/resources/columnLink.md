---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511864"
---
# <a name="columnlink-resource-type"></a>ColumnLink リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。

[contentType]: contenttype.md

## <a name="json-representation"></a>JSON 表記

以下は、**columnLink** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | 列の一意の識別子。
| **name**      | string | このコンテンツ タイプの列の名前。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": [
    "Error: /api-reference/beta/resources/columnLink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
