---
title: imageInfo リソースの種類
description: Activity オブジェクトの visualInfo パーツの**属性**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 53496734f79121edd010a429ec0a8da28b16e836
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008888"
---
# <a name="imageinfo-resource-type"></a>imageInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Activity](../resources/projectrome-activity.md)オブジェクトの[visualinfo](../resources/projectrome-visualinfo.md)パーツの**属性**プロパティを表すための複合型。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|iconUrl | String | オプションアクティビティを生成するために使用されるアプリケーションを表すアイコンを指す URI。|
|alternateText | String | オプションalt キーを押しながら、画像にアクセスできるコンテンツ|
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
