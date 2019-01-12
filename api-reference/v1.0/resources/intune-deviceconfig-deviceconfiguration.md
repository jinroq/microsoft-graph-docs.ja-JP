---
title: deviceConfiguration リソースの種類
description: デバイス構成です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a508a037dbd1271d30a226d9cf62fb0683b53af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953148"
---
# <a name="deviceconfiguration-resource-type"></a>deviceConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス構成です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceConfigurations のリスト](../api/intune-deviceconfig-deviceconfiguration-list.md)|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceConfiguration の取得](../api/intune-deviceconfig-deviceconfiguration-get.md)|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[アクションの割り当て](../api/intune-deviceconfig-deviceconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|説明|String|デバイス構成について管理者が提供した説明です。|
|displayName|String|デバイス構成について管理者が指定した名前です。|
|version|Int32|デバイス構成のバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



