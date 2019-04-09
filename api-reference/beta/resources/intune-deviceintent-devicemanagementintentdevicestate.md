---
title: devicemanagementintentdevicestate リソースの種類
description: 目的のデバイス状態を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2872fa9cccd4f68f274605168689068cf52b157
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522539"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a>devicemanagementintentdevicestate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

目的のデバイス状態を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementIntentDeviceStates](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)コレクション|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementintentdevicestate の取得](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementintentdevicestate の作成](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|新しい[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトを作成します。|
|[devicemanagementintentdevicestate の削除](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|なし|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)を削除します。|
|[devicemanagementintentdevicestate の更新](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ID|
|userPrincipalName|String|デバイスで報告されているユーザープリンシパル名|
|userName|文字列型 (String)|デバイスで報告されているユーザー名|
|deviceDisplayName|String|レポートされているデバイス名|
|lastReportedDateTime|DateTimeOffset|インテントレポートの最終更新日時|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|目的のデバイス状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|deviceId|文字列|レポートされているデバイス id|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```







