---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされる形式は、Windows、およびインターネットに割り当てられた電話番号 (IANA) タイムゾーン (olson タイムゾーンとも呼ばれます)
localization_priority: Normal
ms.openlocfilehash: ced18a28a5c086416fa7247e1531d772fd63b977
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456915"
---
# <a name="timezoneinformation-resource-type"></a>timeZoneInformation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

タイム ゾーンを表します。 サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|alias|string|タイム ゾーンの識別子。|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timezoneinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
