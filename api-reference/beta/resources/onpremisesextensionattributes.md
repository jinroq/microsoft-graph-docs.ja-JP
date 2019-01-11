---
title: onPremisesExtensionAttributes リソースの種類
description: ユーザー エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。 クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。
localization_priority: Normal
ms.openlocfilehash: 44589338e25e01cb483df6bfa3c1e078e352f5ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868160"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ユーザー](user.md)エンティティの**onPremisesExtensionAttributes**プロパティには、15 個のカスタム拡張機能属性のプロパティが含まれています。 このプロパティのセットをオンプレミスの Active Directory のマスターし、Azure AD は、同期**onPremisesSyncEnabled**のユーザーは読み取り専用とします。 クラウド専用 ( **onPremisesSyncEnabled**は false)、ユーザーに対してこれらのプロパティは作成時に設定するか、更新します。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
