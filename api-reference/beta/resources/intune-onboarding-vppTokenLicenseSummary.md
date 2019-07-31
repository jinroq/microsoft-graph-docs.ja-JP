---
title: vppTokenLicenseSummary リソースの種類
description: トークン内の特定のアプリのライセンスの概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20bb4e83d3b69a705c172464fd18df53d1678df7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997989"
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





