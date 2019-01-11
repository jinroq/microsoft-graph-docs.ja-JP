---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6f0d2de25034c28fed12ad8df4caa5e6c3de8506
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837030"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a>deviceConfigurationDeviceOverview リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceConfigurationDeviceOverview](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceConfigurationDeviceOverview](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|pendingCount|Int32|保留中のデバイスの数|
|notApplicableCount|Int32|該当しないデバイスの数|
|notApplicablePlatformCount|Int32|一致していないプラットフォームとポリシーが適用されないデバイスの数|
|successCount|Int32|成功したデバイスの数|
|errorCount|Int32|エラー デバイスの数|
|failedCount|Int32|失敗したデバイスの数|
|conflictCount|Int32|競合しているデバイスの数|
|lastUpdateDateTime|DateTimeOffset|最終更新時刻|
|configurationVersion|Int32|対象の概要に関するポリシーのバージョン|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





