---
title: audioSourceLevel リソースの種類
description: 他のソースのレベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa3a06d319eea0e3af5c016a9ef799591f76fabb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013214"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

他のソースのレベルの構成。

## <a name="properties"></a>プロパティ

| プロパティ               | 型    | 説明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| その他のウィ氏             | Boolean | このソースが、アクティブな他のソースをアヒルに使用できるようにします。 True に設定する場合は、ducking level を設定する必要があります。|
| level                  | Int64   | Ducking がに`true`設定され`duckOthers`ている場合のソースのレベル。                                     |
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
