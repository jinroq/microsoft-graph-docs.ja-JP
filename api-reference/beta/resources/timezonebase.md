---
title: timeZoneBase リソースの種類
description: タイム ゾーンの基本的な表現です。
ms.openlocfilehash: 00e09b064a083aa72316838c213f9c84e1139a19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073144"
---
# <a name="timezonebase-resource-type"></a>timeZoneBase リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

タイム ゾーンの基本的な表現です。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| name | 文字列 | タイム ゾーンの名前。 標準的なタイム ゾーンの名前 ("ハワイ アリューシャン標準時" など) を使用することも、カスタム タイム ゾーンとして "カスタム タイム ゾーン" という名前を指定することもできます。 |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->