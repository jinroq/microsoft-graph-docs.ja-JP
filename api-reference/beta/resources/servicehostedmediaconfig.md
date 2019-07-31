---
title: serviceHostedMediaConfig リソースの種類
description: ServiceHostedMediaConfig の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f56928a7294fba1cb31f5061a2c7b8f7bb70f02a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965202"
---
# <a name="servicehostedmediaconfig-resource-type"></a>serviceHostedMediaConfig リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ServiceHostedMediaConfig の種類。

## <a name="properties"></a>プロパティ

| プロパティ                    | 型                                                        | 説明                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| preFetchMedia               | [mediaInfo](mediainfo.md)コレクション                        | 事前にフェッチするメディアのリスト。                   |
| removeFromDefaultAudioGroup | Boolean                                                     | 既定のオーディオグループから自分の参加者を削除します。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a>例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
