---
title: parentalControlSettings リソースの種類
description: アプリケーションにおける、保護者による制限設定を指定します。 これらの設定は、同意の操作性を制御します。
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643004"
---
# <a name="parentalcontrolsettings-resource-type"></a>parentalControlSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションにおける、保護者による制限設定を指定します。 これらの設定は、同意の操作性を制御します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String コレクション| [2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。 アプリケーションへのアクセスは、このリストで指定した国からの未成年者がブロックされます。|
|legalAgeGroupRule| String | アプリケーションのユーザーに適用される法律の年齢グループの規則を指定します。 次の値のいずれかに設定できます。 <table><tr><th>値</th><th>説明</th></tr><tr><td>Allow</td><td>既定値。 有効な最小値を適用します。 これは、保護者の同意は、欧州連合と韓国で未成年者に必要なことを意味します。</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>COPPA の規則に準拠する誕生日の日付を指定するユーザーを強制します。 </td></tr><tr><td>RequireConsentForMinors</td><td>下国のマイナー ルールに関係なく、18 歳の保護者の同意が必要です。</td></tr><tr><td>RequireConsentForKids</td><td>下国のマイナー ルールに関係なく、14 歳の保護者の同意が必要です。</td></tr><tr><td>BlockMinors</td><td>アプリケーションを使用してから未成年をブロックします。</td></tr></table> |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
