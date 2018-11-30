---
title: synchronizationError リソースの種類
description: 同期処理中に発生したエラーを表します。
ms.openlocfilehash: a1e3725151a4e36772cd3b6079f787370f4c85dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067251"
---
# <a name="synchronizationerror-resource-type"></a>synchronizationError リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

同期処理中に発生したエラーを表します。

## <a name="properties"></a>プロパティ

<!-- Add descriptions for the properties. -->
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|code|String||
|message|String||
|tenantActionable|ブール値||

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->