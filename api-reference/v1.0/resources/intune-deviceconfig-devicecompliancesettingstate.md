---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
ms.openlocfilehash: e4edce4b22b70c6018703e086d606b84781b6b91
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326174"
---
# <a name="devicecompliancesettingstate-resource-type"></a>deviceComplianceSettingState リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceComplianceSettingStates](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。|
|[Delete deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|なし|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。|
|[Update deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー|
|setting|String|設定のクラス名とプロパティ名。|
|settingName|String|レポートされている設定名。|
|deviceId|String|レポートされているデバイス ID。|
|deviceName|String|レポートされているデバイス名。|
|userId|String|レポートされているユーザー ID|
|userEmail|String|レポートされているユーザーのメール アドレス。|
|userName|String|レポートされているユーザー名|
|userPrincipalName|String|レポートされているユーザーの PrincipalName|
|deviceModel|String|レポートされているデバイス モデル|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|設定のコンプライアンスの状態です。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎる DateTime|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



