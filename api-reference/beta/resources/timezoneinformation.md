---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされている形式は、Windows、およびインターネット割り当て番号機関 (IANA) はタイム ゾーン (Olson タイム ・ ゾーンとも呼ばれます)
localization_priority: Normal
ms.openlocfilehash: dc53cca34ef9c6a53a39394cbba8be4e1baca662
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839740"
---
# <a name="timezoneinformation-resource-type"></a>timeZoneInformation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

タイム ゾーンを表します。 サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|alias|文字列|タイム ゾーンの識別子。|
|displayName|string|タイム ゾーンを表す表示文字列。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
