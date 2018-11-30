---
title: onenoteOperation リソースの種類
description: OneNote の特定の長時間操作の状態。
ms.openlocfilehash: af7da970a148d4b70385487503e3abf6431c430a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067559"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

OneNote の特定の長時間操作の状態。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |操作の開始時刻です。|
|error|[onenoteOperationError](onenoteoperationerror.md)|操作によって返されるエラーです。|
|ID|文字列|操作 ID です。読み取り専用です。|
|lastActionDateTime| DateTimeOffset |操作の最後の操作の時間です。|
|resourceId|文字列|リソース ID。|
|resourceLocation|文字列|オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。 |
|status|文字列|操作の現在の状態: `notstarted`、`running`、`completed`、`failed` |
|percentComplete|文字列|操作がまだ `running` の状態の場合の操作達成率。

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[操作の取得](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |操作の現在の状態を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
