---
title: configurationManagerClientHealthState リソースの種類
description: 構成マネージャー クライアントの正常性状態
ms.openlocfilehash: f2724f5d230ee539720e105daf1758bf727bee26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067852"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>configurationManagerClientHealthState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

構成マネージャー クライアントの正常性状態
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|現在の構成マネージャー クライアントの状態です。 可能な値は、`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError` です。|
|errorCode|Int32|障害状態のエラー コード。|
|lastSyncDateTime|DateTimeOffset|Datetime/fo オプション最後の同期の構成マネージャーの管理をポイントします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





