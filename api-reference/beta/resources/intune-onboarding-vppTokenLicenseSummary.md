---
title: vppTokenLicenseSummary リソースの種類
description: トークン内の特定のアプリのライセンスの概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b80b5b1d8db1d2352f32413ff4a03b9279cd8b7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958614"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

トークン内の特定のアプリのライセンスの概要。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|vppTokenId|String|VPP トークンの識別子。|
|appleId|String|特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。|
|organizationName|String|Apple Volume Purchase Program のトークンに関連付けられている組織。|
|availableLicenseCount|Int32|使用可能な VPP ライセンスの数。|
|usedLicenseCount|Int32|使用中の VPP ライセンスの数。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```





