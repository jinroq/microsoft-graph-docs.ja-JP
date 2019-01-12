---
title: domainState リソースの種類
description: ドメイン上でスケジュールされている非同期操作の状態を表します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6a7741448b9c91be32f67f89cbafa5a579320083
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938294"
---
# <a name="domainstate-resource-type"></a>domainState リソースの種類

ドメイン上でスケジュールされている非同期操作の状態を表します。

## <a name="properties"></a>プロパティ

| プロパティ   | 種類 | 説明 |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | 最後のアクティビティが発生したときのタイムスタンプ。値は、操作のスケジュール時、非同期タスクの開始時、操作の完了時に更新されます。 |
| 操作​​ | String | 非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。 |
| status | String | 操作の現在の状態。 <br> *Scheduled* - 操作はスケジュールされていますが、開始されていません。 <br> *InProgress* - タスクが開始され、実行中です。 <br> *Failed* - 操作が失敗しました。 |

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
