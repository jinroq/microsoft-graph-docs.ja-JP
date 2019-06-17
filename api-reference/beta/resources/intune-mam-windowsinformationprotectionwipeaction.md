---
title: Windowsinformationprotectionwipepeaction リソースの種類
description: テナント管理者が独自のデバイス (BYOD) Windows デバイス用に発行したワイプ要求を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dccbc89b38abd00a9b464f82cc0531e6fbab47ab
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994399"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>Windowsinformationprotectionwipepeaction リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナント管理者が独自のデバイス (BYOD) Windows デバイス用に発行したワイプ要求を表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsInformationProtectionWipeActions を一覧表示する](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション|[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsInformationProtectionWipeAction を取得する](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsInformationProtectionWipeAction を作成する](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|新しい[Windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。|
|[WindowsInformationProtectionWipeAction を削除する](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|None|[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。|
|[WindowsInformationProtectionWipeAction を更新する](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|status|[actionState](../resources/intune-shared-actionstate.md)|ワイプアクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|targetedUserId|String|このワイプアクションの対象となる UserId。|
|targetedDeviceRegistrationId|String|このワイプアクションの対象となる DeviceRegistrationId。|
|targetedDeviceName|String|対象のデバイス名。|
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





