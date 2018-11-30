---
title: imageInfo リソースの種類
description: アクティビティ オブジェクトの visualInfo の一部の**属性**のプロパティを表すための複合型です。
ms.openlocfilehash: 051338230850da7e754c5e8ad4f7d9c52fe17b32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023140"
---
# <a name="imageinfo-resource-type"></a>imageInfo リソースの種類

[アクティビティ](../resources/projectrome-activity.md)オブジェクトの[visualInfo](../resources/projectrome-visualinfo.md)の一部の**属性**のプロパティを表すための複合型です。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|iconUrl | String | 省略可能です。活動を生成するために使用するアプリケーションを表すアイコンをポイントする URI|
|alternateText | String | 省略可能です。イメージの alt テキストのアクセス可能なコンテンツ|
|addImageQuery | ブール値 | 省略可能です。サーバーを指定するためのパラメーターは、パラメーターへの応答に動的にイメージをレンダリングすることです。 例: ハイコントラスト イメージ|

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
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->