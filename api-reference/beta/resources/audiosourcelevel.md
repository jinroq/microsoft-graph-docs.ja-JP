---
title: audioSourceLevel リソースの種類
description: 他のソースのレベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535596"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

他のソースのレベルの構成。

## <a name="properties"></a>プロパティ

| プロパティ               | 型    | 説明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| その他のウィ氏             | ブール値 | このソースが、アクティブな他のソースをアヒルに使用できるようにします。 true に設定する場合は、ducking level を設定する必要があります。|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
