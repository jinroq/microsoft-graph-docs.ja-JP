---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b62a44e34ca19b80c35062c884c00fd5ceeaeb38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919261"
---
# <a name="iosvppappassignmentsettings-resource-type"></a>iosVppAppAssignmentSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。

[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|useDeviceLicensing|ブール型 (Boolean)|デバイスのライセンスを使用するかどうか。|
|vpnConfigurationId|文字列型 (String)|このアプリに適用するための VPN 構成 ID。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```





