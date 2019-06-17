---
title: deviceCompliancePolicySettingStateSummary リソースの種類
description: アカウント全体における、デバイス コンプライアンスのポリシー設定状態の要約です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9aef48828c9a774074ffe7396189dc4aad98e700
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995498"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>deviceCompliancePolicySettingStateSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|setting|String|設定のクラス名とプロパティ名。|
|settingName|String|設定の名前。|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|プラットフォームを設定します。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。|
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





