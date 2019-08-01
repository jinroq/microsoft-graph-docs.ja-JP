---
title: domainState リソースの種類
description: ドメインでスケジュールされた非同期操作の状態を表します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: feefe750997735d9f814f425ffd1380e25800a30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029415"
---
# <a name="domainstate-resource-type"></a>domainState リソースの種類

ドメインでスケジュールされた非同期操作の状態を表します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | 最後のアクティビティが発生したときのタイムスタンプ。 この値は、操作がスケジュールされたとき、非同期タスクが開始されたとき、および操作が完了したときに更新されます。 |
| operation | String | 非同期操作の種類。 指定できる値は、 *Forcedelete*または*ベリファイ*です |
| status | String | 操作の現在の状態。 <br> *スケジュール*済み-操作はスケジュールされていますが、開始されていません。 <br> *InProgress* -タスクが開始され、進行中です。 <br> *失敗*-操作が失敗しました。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
