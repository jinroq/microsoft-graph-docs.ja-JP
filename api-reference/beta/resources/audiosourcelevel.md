---
title: audioSourceLevel リソースの種類
description: 他のソースのレベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc2b0c11b18a3cf8120cab0bb9c745ae8880cfc6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339064"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

他のソースのレベルの構成。

## <a name="properties"></a>プロパティ

| プロパティ               | 型    | 説明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| その他のウィ氏             | Boolean | このソースが、アクティブな他のソースをアヒルに使用できるようにします。 true に設定する場合は、ducking level を設定する必要があります。|
| 大まか                  | Int64   | Ducking がに`true`設定され`duckOthers`ている場合のソースのレベル。                                     |
| 積極的            | String  | ソース参加者のオーディオストリーム。                                                                |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
