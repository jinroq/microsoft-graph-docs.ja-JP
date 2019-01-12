---
title: audioDuckingConfiguration リソースの種類
description: ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916874"
---
# <a name="audioduckingconfiguration-resource-type"></a>audioDuckingConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター

## <a name="properties"></a>プロパティ

| プロパティ      | 種類     | 説明                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | % のソースを ducked されているときに元のボリューム。             |
| rampActive    | Int64    | Ducked ソースの「フェードアウト」にかかる時間 (ミリ秒単位) の量。 |
| rampInactive  | Int64    | Ducked ソースの「フェードイン」にかかる時間 (ミリ秒単位) の量。  |
| upperLevel    | Int64    | % のソースは ducked されていないときに元のボリューム。         |

> **注:** ランプの期間は、5,000 人以上のミリ秒になることはできません。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
