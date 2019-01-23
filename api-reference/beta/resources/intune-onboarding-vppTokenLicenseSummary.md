---
title: vppTokenLicenseSummary リソースの種類
description: トークンで指定されたアプリケーションのライセンスの概要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395182"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

トークンで指定されたアプリケーションのライセンスの概要です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|vppTokenId|String|VPP トークンの識別子です。|
|appleId|String|特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。|
|organizationName|String|Apple ボリューム購入プログラム トークンに関連付けられている組織です。|
|availableLicenseCount|Int32|VPP のライセンスが使用可能な数です。|
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




