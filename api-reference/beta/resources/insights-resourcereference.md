---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520005"
---
# <a name="resourcereference-resource-type"></a>resourceReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複合型のプロパティ[情報](insights.md)にはが含まれています。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明  |
| ------------- |-----------| -------------|
| webUrl        | String    | 参照先の項目に先行する URL です。 |
| id            | String    | アイテムの一意の識別子です。           |
| type          | String    | 文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
