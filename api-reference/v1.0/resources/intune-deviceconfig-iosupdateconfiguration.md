---
title: iosUpdateConfiguration リソースの種類
description: iOS 更新構成では、iOS の更新をインストールする、一週間のうちの時間枠を構成できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9eafeab5f7aa2be9c0007d989cfb63fc0aad174
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028183"
---
# <a name="iosupdateconfiguration-resource-type"></a>iosUpdateConfiguration リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS 更新構成では、iOS の更新をインストールする、一週間のうちの時間枠を構成できます。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosUpdateConfigurations のリスト](../api/intune-deviceconfig-iosupdateconfiguration-list.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) コレクション|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosUpdateConfiguration の取得](../api/intune-deviceconfig-iosupdateconfiguration-get.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosUpdateConfiguration の作成](../api/intune-deviceconfig-iosupdateconfiguration-create.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|新しい [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを作成します。|
|[iosUpdateConfiguration の削除](../api/intune-deviceconfig-iosupdateconfiguration-delete.md)|なし|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) を削除します。|
|[iosUpdateConfiguration の更新](../api/intune-deviceconfig-iosupdateconfiguration-update.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|activeHoursStart|TimeOfDay|アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)|
|activeHoursEnd|TimeOfDay|アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)|
|scheduledInstallDays|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)コレクション|アクティブ時間が設定されている曜日。 このコレクションには、最大で 7 個の要素を含めることができます。|
|utcTimeOffsetInMinutes|Int32|分単位で示す、UTC タイム オフセット|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-deviceconfig-iosupdateconfiguration.md/microsoft.graph.iosUpdateConfiguration/scheduledInstallDays:
     Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


