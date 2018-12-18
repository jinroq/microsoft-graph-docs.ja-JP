---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。
author: tfitzmac
ms.openlocfilehash: d502af67cc1a68c56e1bdd74965e77224947b5d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344633"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsAutopilotSettings を取得します。](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsAutopilotSettings を更新します。](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。|
|[同期アクション](../api/intune-enrollment-windowsautopilotsettings-sync.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|オブジェクトの GUID|
|lastSyncDateTime|DateTimeOffset|最後のデータは、DDS のサービスでの日付の時刻を同期します。|
|lastManualSyncTriggerDateTime|DateTimeOffset|最後のデータは、DDS のサービスでの日付の時刻を同期します。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|デバイスのデータ同期 (DDS) のサービスとの同期のステータスを示します。 可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```





