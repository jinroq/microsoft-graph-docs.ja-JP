---
title: parentalcontrolsettings リソースの種類
description: アプリケーションにおける、保護者による制限設定を指定します。 これらの設定は、同意操作を制御します。
localization_priority: Normal
ms.openlocfilehash: 8e62e137b872437626a5c77c114f14c6ad0c5eb2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344994"
---
# <a name="parentalcontrolsettings-resource-type"></a>parentalcontrolsettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションにおける、保護者による制限設定を指定します。 これらの設定は、同意操作を制御します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String collection| [2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。 この一覧で指定された国からの未成年者では、アプリケーションへのアクセスがブロックされます。|
|legalAgeGroupRule| String | アプリのユーザーに適用する法的年齢グループルールを指定します。 以下のいずれかの値に設定できます。 <table><tr><th>値</th><th>説明</th></tr><tr><td>許可</td><td>既定値です。 リーガルの最小値を強制します。 これは、欧州連合と韓国の未成年者について、キッズセーフティが必要であることを意味します。</td></tr><tr><td>requireconforprivacyservices</td><td>ユーザーが COPPA ルールに準拠する生年月日を指定することを強制します。 </td></tr><tr><td>requireconforminor</td><td>国のマイナールールに関係なく、18才以下の年齢に対しては、上位下位の同意が必要です。</td></tr><tr><td>requireconforkids</td><td>国のマイナールールに関係なく、14才未満の年齢に対して上位下位の同意が必要です。</td></tr><tr><td>BlockMinors</td><td>未成年者がアプリを使用することをブロックします。</td></tr></table> |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
