---
title: windowsinformationprotectionwipepeaction リソースの種類
description: テナント管理者が独自のデバイス (byod) Windows デバイス用に発行したワイプ要求を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e08cd6a2cf27830f6f88328440fb100bcd77ef6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148007"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>windowsinformationprotectionwipepeaction リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナント管理者が独自のデバイス (byod) Windows デバイス用に発行したワイプ要求を表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsinformationprotectionwipeactions を一覧表示する](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション|[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsinformationprotectionwipeaction を取得する](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsinformationprotectionwipeaction を作成する](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|新しい[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。|
|[windowsinformationprotectionwipeaction を削除する](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|なし|[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。|
|[windowsinformationprotectionwipeaction を更新する](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|status|[actionState](../resources/intune-shared-actionstate.md)|ワイプアクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|targeteduserid|String|このワイプアクションの対象となる UserId。|
|targetedDeviceRegistrationId|String|このワイプアクションの対象となる DeviceRegistrationId。|
|targeteddevicename|String|対象のデバイス名。|
|targetedDeviceMacAddress|String|対象デバイスの Mac アドレス。|
|lastCheckInDateTime|DateTimeOffset|このワイプアクションの対象となったデバイスの最終チェックイン時刻。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




