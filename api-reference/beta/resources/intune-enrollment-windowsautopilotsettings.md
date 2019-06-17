---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、windows device data sync service とデータを同期する Windows 自動操縦アカウントを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7bbdfa28061b48a0c2ca3ed2e0b714e1f1a1159
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989715"
---
# <a name="windowsautopilotsettings-resource-type"></a>windowsAutopilotSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

WindowsAutopilotSettings リソースは、windows device data sync service とデータを同期する Windows 自動操縦アカウントを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsAutopilotSettings を取得する](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsAutopilotSettings の更新](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。|
|[同期アクション](../api/intune-enrollment-windowsautopilotsettings-sync.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|lastSyncDateTime|DateTimeOffset|DDS サービスによる最終データ同期日時。|
|lastManualSyncTriggerDateTime|DateTimeOffset|DDS サービスによる最終データ同期日時。|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|デバイスデータ同期 (DDS) サービスとの同期の状態を示します。 可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。|

## <a name="relationships"></a>リレーションシップ
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





