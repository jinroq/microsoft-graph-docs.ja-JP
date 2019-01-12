---
title: deviceCompliancePolicySettingStateSummary リソースの種類
description: アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 73c5ad3df2b768d9cc1888de714876a2c963562e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914872"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>deviceCompliancePolicySettingStateSummary リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCompliancePolicySettingStateSummaries のリスト](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceCompliancePolicySettingStateSummary の取得](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceCompliancePolicySettingStateSummary の作成](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。|
|[deviceCompliancePolicySettingStateSummary の削除](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|なし|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) を削除します。|
|[deviceCompliancePolicySettingStateSummary の更新](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|setting|String|設定のクラス名とプロパティ名。|
|settingName|String|設定の名前。|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|設定のプラットフォームです。 可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。|
|unknownDeviceCount|Int32|不明なデバイスの数|
|notApplicableDeviceCount|Int32|該当しないデバイスの数|
|compliantDeviceCount|Int32|準拠デバイスの数|
|remediatedDeviceCount|Int32|修復済みデバイスの数|
|nonCompliantDeviceCount|Int32|準拠していないデバイスの数|
|errorDeviceCount|Int32|エラー デバイスの数|
|conflictDeviceCount|Int32|競合デバイスの数|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション|まだ文書化されていません|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



