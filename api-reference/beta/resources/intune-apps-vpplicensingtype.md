---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
ms.openlocfilehash: 83e68cc018b3e3f5948b105118bffbeb93010c2f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351304"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|supportUserLicensing|ブール型 (Boolean)|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
|supportDeviceLicensing|ブール型 (Boolean)|プログラムがデバイス ライセンスの種類をサポートするかどうか。|
|supportsUserLicensing|ブール型 (Boolean)|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
|supportsDeviceLicensing|ブール型 (Boolean)|プログラムがデバイス ライセンスの種類をサポートするかどうか。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





