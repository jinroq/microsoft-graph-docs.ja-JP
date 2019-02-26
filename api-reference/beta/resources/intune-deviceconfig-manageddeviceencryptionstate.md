---
title: manageddeviceencryptionstate リソースの種類
description: デバイスごとの暗号化レポート
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee73ab13ea48707eed745bced197fdd7ae5676b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177848"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>manageddeviceencryptionstate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスごとの暗号化レポート

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[manageddeviceencryptionstates のリスト](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)コレクション|[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[manageddeviceencryptionstate の取得](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[manageddeviceencryptionstate の作成](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|新しい[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを作成します。|
|[manageddeviceencryptionstate の削除](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|なし|[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)を削除します。|
|[manageddeviceencryptionstate の更新](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userPrincipalName|文字列|ユーザー名|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|デバイスのプラットフォーム。 可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|osVersion|String|デバイスのオペレーティングシステムのバージョン|
|tpmSpecificationVersion|String|デバイス TPM のバージョン|
|deviceName|String|デバイス名|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|暗号化の準備状態。 使用可能な値は、`notReady`、`ready` です。|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|デバイスの暗号化の状態。 使用可能な値は、`notEncrypted`、`encrypted` です。|
|encryptionpolicysettingstate|[complianceStatus](../resources/intune-shared-compliancestatus.md)|暗号化ポリシーの設定状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|advanced bitlockerstates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|高度な BitLocker 状態。 可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`|
|policydetails|[encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション|ポリシーの詳細|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```




