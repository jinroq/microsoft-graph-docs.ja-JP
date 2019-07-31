---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされる形式は、Windows、およびインターネットに割り当てられた電話番号 (IANA) タイムゾーン (Olson タイムゾーンとも呼ばれます)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea20a14ddd18e533767e7e969a91a07f6e2ad479
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964287"
---
# <a name="timezoneinformation-resource-type"></a>timeZoneInformation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

タイム ゾーンを表します。 サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|エイリアス|string|タイム ゾーンの識別子。|
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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
