---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 4a07c879e20139c9138fc7315172655aa48a40eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021552"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|デバイスがチェックインせずに移動し、準拠性を維持できる日数です。 有効な値は 0 から 120 までです|
|isScheduledActionEnabled|Boolean|ルールのスケジュール済みアクションの機能が有効かどうか。|
|secureByDefault|Boolean|これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



