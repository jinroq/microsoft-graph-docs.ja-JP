---
title: mediaStream リソースの種類
description: MediaStream の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c39c4eb0754f327361fec04852293ef084b0c412
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966827"
---
# <a name="mediastream-resource-type"></a>mediaStream リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

MediaStream の種類。

## <a name="properties"></a>プロパティ

| プロパティ    | 型    | 説明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | 方向を示します。 使用可能な値`inactive`は`sendOnly` `receiveOnly`、、 `sendReceive`、です。                  |
| label       | String  | メディアストリームのラベル。                                                                                       |
| mediaType   | String  | メディアの種類。 使用可能な値`unknown`は`audio` `video` `videoBasedScreenSharing`、、、 `data`、です。        |
| serverMuted | Boolean | メディアがサーバーによってミュートされている場合。                                                                          |
| sourceId    | String  | ソース ID。                                                                                                |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a>例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
