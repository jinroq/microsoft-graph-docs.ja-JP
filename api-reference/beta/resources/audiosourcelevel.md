---
title: audioSourceLevel リソースの種類
description: その他のソース レベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: adf3c4805271d0a8d02d25fc8e7ecb547db10215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880641"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

その他のソース レベルの構成。

## <a name="properties"></a>プロパティ

| プロパティ               | 種類    | 説明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | ブール型 | Duck のアクティブなときに他のソースには、このソースを有効にします。 レベルをかわす、true に設定を設定する場合。|
| level                  | Int64   | 場合に、ソースのレベルをかわす`duckOthers`に設定されて`true`。                                     |
| 参加者            | String  | ソースの参加者オーディオ ストリームです。                                                                |

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
