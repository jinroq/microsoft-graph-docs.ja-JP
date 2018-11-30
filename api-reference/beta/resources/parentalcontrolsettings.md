---
title: parentalControlSettings リソースの種類
description: アプリケーションの視聴制限の設定を指定します。 これらの設定は、同意の操作性を制御します。
ms.openlocfilehash: 96f0fa96f9257187e404b61eaca877302d50ccee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067389"
---
# <a name="parentalcontrolsettings-resource-type"></a>parentalControlSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーションの視聴制限の設定を指定します。 これらの設定は、同意の操作性を制御します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String コレクション| [2 文字の ISO 国コード](https://www.iso.org/iso-3166-country-codes.html)を指定します。 アプリケーションへのアクセスは、このリストで指定した国からの未成年者がブロックされます。|
|legalAgeGroupRule| String | アプリケーションのユーザーに適用される法律の年齢グループの規則を指定します。 次の値のいずれかに設定できます。 <table><tr><th>値</th><th>説明</th></tr><tr><td>Allow</td><td>既定値です。 有効な最小値を適用します。 これは、保護者の同意は、欧州連合と韓国で未成年者に必要なことを意味します。</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>COPPA の規則に準拠する誕生日の日付を指定するユーザーを強制します。 </td></tr><tr><td>RequireConsentForMinors</td><td>下国のマイナー ルールに関係なく、18 歳の保護者の同意が必要です。</td></tr><tr><td>RequireConsentForKids</td><td>下国のマイナー ルールに関係なく、14 歳の保護者の同意が必要です。</td></tr><tr><td>BlockMinors</td><td>アプリケーションを使用してから未成年をブロックします。</td></tr></table> |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
