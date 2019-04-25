---
title: vpptokenlicensesummary リソースの種類
description: トークン内の特定のアプリのライセンスの概要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1292caa41a2e56c42adde8be7f9bb8988b369cd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566410"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vpptokenlicensesummary リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

トークン内の特定のアプリのライセンスの概要。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|vppTokenId|String|VPP トークンの識別子。|
|appleId|String|特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。|
|organizationName|String|Apple volume purchase program のトークンに関連付けられている組織。|
|availableLicenseCount|Int32|使用可能な VPP ライセンスの数。|
|usedLicenseCount|Int32|使用中の VPP ライセンスの数。|

## <a name="relationships"></a>関係
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





