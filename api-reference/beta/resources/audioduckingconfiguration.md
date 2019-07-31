---
title: Audioアヒルの構成リソースの種類
description: 他のソースの ducking のパラメーター (他のソースの段階的なインおよび out)。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cfff0ca240a13c9c4396d605def05a52e1916778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013221"
---
# <a name="audioduckingconfiguration-resource-type"></a>Audioアヒルの構成リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

他のソースの ducking のパラメーター (他のソースの段階的なインおよび out)。

## <a name="properties"></a>プロパティ

| プロパティ      | 型     | 説明                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| 下位レベル    | Int64    | ソースが処理されるときのソースの量 (パーセント)。             |
| rampActive    | Int64    | 発行元が "フェードアウト" するまでにかかる時間 (ミリ秒)。 |
| rampInactive  | Int64    | 発行元が "フェードイン" になるまでにかかる時間 (ミリ秒)。  |
| upperLevel    | Int64    | ソースが発行されていない場合のソースの量 (パーセント)。         |

> **注:** 傾斜時間は5000ミリ秒を超えることはできません。

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
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
