---
title: mediaStream リソースの種類
description: MediaStream 型です。
author: VinodRavichandran
ms.openlocfilehash: f870611700289f0254272b78e18e344d02dd123e
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380297"
---
# <a name="mediastream-resource-type"></a>mediaStream リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

MediaStream 型です。

## <a name="properties"></a>プロパティ

| プロパティ    | 型    | 説明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| 方向   | String  | 方向です。 使用可能な値は、 `inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。                  |
| label       | String  | メディア ストリームのラベルです。                                                                                       |
| メディアの種類   | String  | メディアは次のとおり入力します。 使用可能な値は、 `unknown`、 `audio`、 `video`、 `videoBasedScreenSharing`、 `data`。        |
| serverMuted | Boolean | サーバによってメディアがミュートされている場合。                                                                          |
| sourceId    | String  | ソースの id。                                                                                                |

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
