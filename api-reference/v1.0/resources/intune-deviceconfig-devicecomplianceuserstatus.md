---
title: deviceComplianceUserStatus リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 48a491ee8e7c3ef6e31171725376bf735f3e12d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934899"
---
# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
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



