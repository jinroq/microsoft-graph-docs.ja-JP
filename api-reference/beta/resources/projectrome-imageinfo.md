---
title: imageInfo リソースの種類
description: activity オブジェクトの visualinfo パーツの**属性**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6ffdacefb11f583f8c9529a36472a01537643c3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344010"
---
# <a name="imageinfo-resource-type"></a>imageInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[activity](../resources/projectrome-activity.md)オブジェクトの[visualinfo](../resources/projectrome-visualinfo.md)パーツの**属性**プロパティを表すための複合型。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|iconUrl | String | オプションアクティビティを生成するために使用されるアプリケーションを表すアイコンを指す URI。|
|alternatetext | String | オプションalt キーを押しながら、画像にアクセスできるコンテンツ|
|addImageQuery | Boolean | オプションパラメータパラメーターへの応答として、サーバーが画像を動的に表示できることを示すために使用されます。 例-コントラストの高い画像|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
