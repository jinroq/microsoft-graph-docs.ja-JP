---
title: deviceComplianceUserStatus リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3da7aa139918b08006a7a8398f92b18b2687c29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031641"
---
# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceComplianceUserStatuses のリスト](../api/intune-deviceconfig-devicecomplianceuserstatus-list.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) コレクション|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceComplianceUserStatus の取得](../api/intune-deviceconfig-devicecomplianceuserstatus-get.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceComplianceUserStatus の作成](../api/intune-deviceconfig-devicecomplianceuserstatus-create.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|新しい [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを作成します。|
|[deviceComplianceUserStatus の削除](../api/intune-deviceconfig-devicecomplianceuserstatus-delete.md)|なし|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) を削除します。|
|[deviceComplianceUserStatus の更新](../api/intune-deviceconfig-devicecomplianceuserstatus-update.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|userDisplayName|String|DevicePolicyStatus のユーザー名。|
|devicesCount|Int32|そのユーザーのデバイスの数。|
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
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



