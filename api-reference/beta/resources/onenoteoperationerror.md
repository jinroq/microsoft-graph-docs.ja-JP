---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
ms.openlocfilehash: 0dab8b405c99f2931d2cc02cc915df5f805322d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073069"
---
# <a name="onenoteoperationerror-resource-type"></a>onenoteOperationError リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

失敗した OneNote 操作によるエラー。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|code|文字列|エラー コード。|
|message|文字列|エラー メッセージ。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
