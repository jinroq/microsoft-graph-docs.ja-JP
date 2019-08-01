---
title: deviceComplianceDeviceStatus リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b20f331b6149ee3f346a869dda25c8931f80dfca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028505"
---
# <a name="devicecompliancedevicestatus-resource-type"></a>deviceComplianceDeviceStatus リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceComplianceDeviceStatuses のリスト](../api/intune-deviceconfig-devicecompliancedevicestatus-list.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) コレクション|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceComplianceDeviceStatus の取得](../api/intune-deviceconfig-devicecompliancedevicestatus-get.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceComplianceDeviceStatus の作成](../api/intune-deviceconfig-devicecompliancedevicestatus-create.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|新しい [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを作成します。|
|[deviceComplianceDeviceStatus の削除](../api/intune-deviceconfig-devicecompliancedevicestatus-delete.md)|なし|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) を削除します。|
|[deviceComplianceDeviceStatus の更新](../api/intune-deviceconfig-devicecompliancedevicestatus-update.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|deviceDisplayName|String|DevicePolicyStatus のデバイス名。|
|userName|文字列型 (String)|レポートされているユーザー名|
|deviceModel|String|レポートされているデバイス モデル|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎる DateTime|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|ポリシー レポートのコンプライアンスの状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|lastReportedDateTime|DateTimeOffset|ポリシー レポートの最終変更日時。|
|userPrincipalName|String|UserPrincipalName。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



