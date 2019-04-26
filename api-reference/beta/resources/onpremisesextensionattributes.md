---
title: onPremisesExtensionAttributes リソースの種類
description: user エンティティの**onPremisesExtensionAttributes**プロパティには、15個のカスタム拡張属性プロパティが含まれています。 **onPremisesSyncEnabled**ユーザーの場合、このプロパティのセットはオンプレミスの Active Directory でマスターされ、Azure AD に同期され、読み取り専用になります。 クラウドのみのユーザー ( **onPremisesSyncEnabled**が false) の場合、これらのプロパティは作成時または更新時に設定できます。
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568893"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[user](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15個のカスタム拡張属性プロパティが含まれています。 **onPremisesSyncEnabled**ユーザーの場合、このプロパティのセットはオンプレミスの Active Directory でマスターされ、Azure AD に同期され、読み取り専用になります。 クラウドのみのユーザー ( **onPremisesSyncEnabled**が false) の場合、これらのプロパティは作成時または更新時に設定できます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|extensionAttribute1|String| 最初のカスタマイズ可能な拡張属性。 |
|extensionAttribute2|String| 2番目のカスタマイズ可能な拡張属性。 |
|extensionAttribute3|String| 3番目のカスタマイズ可能な拡張属性。 |
|extensionAttribute4|String| 4番目のカスタマイズ可能な拡張属性。 |
|extensionAttribute5|String| 5番目のカスタマイズ可能な拡張属性。 |
|extensionAttribute6|String| 6番目のカスタマイズ可能な拡張属性。 |
|extensionAttribute7|String| 7番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute8|String| 8番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute9|String| 9番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute10|String| 10番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute11|String| 11番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute12|String| 12番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute13|String| 13番目にカスタマイズ可能な拡張属性。 |
|extensionAttribute14|String| 14番目のカスタマイズ可能な拡張属性。 |
|extensionAttribute15|String| 15番目のカスタマイズ可能な拡張属性。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
