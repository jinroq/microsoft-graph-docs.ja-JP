---
title: onPremisesExtensionAttributes リソースの種類
description: ユーザー エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 onPremisesSyncEnabled ユーザーの場合、このプロパティ セットはオンプレミスの Active Directory でマスター管理され、Azure AD に同期され、読み取り専用となります。 クラウド専用ユーザー (onPremisesSyncEnabled が false) の場合、これらのプロパティは作成時または更新時に設定される可能性があります。
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518241"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ユーザー](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 onPremisesSyncEnabled ユーザーの場合、このプロパティ セットはオンプレミスの Active Directory でマスター管理され、Azure AD に同期され、読み取り専用となります。 クラウド専用ユーザー (onPremisesSyncEnabled が false) の場合、これらのプロパティは作成時または更新時に設定される可能性があります。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|extensionAttribute1|String| 最初の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute2|String| 2 つ目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute3|String| 3 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute4|String| 4 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute5|String| 5 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute6|String| 6 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute7|String| 7 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute8|String| 8 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute9|String| 9 番目の拡張機能のカスタマイズ可能な属性です。 |
|extensionAttribute10|String| 10 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute11|String| 11 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute12|String| 12 番目にカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute13|String| 13 番目にカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute14|String| 14 番目にカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute15|String| 15 番目のカスタマイズ可能な拡張機能の属性です。 |

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
