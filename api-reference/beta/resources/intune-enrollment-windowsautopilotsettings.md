---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd4641258dbc02829d4b06817467a652de2cb583
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393740"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsAutopilotSettings を取得します。](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsAutopilotSettings を更新します。](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。|
|[同期アクション](../api/intune-enrollment-windowsautopilotsettings-sync.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
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




