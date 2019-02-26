---
title: bitlockersystemdrive policy リソースの種類
description: BitLocker 暗号化の基本ポリシー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27b4492dd6df2821cfdeb885d3412536c0d3991c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164891"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>bitlockersystemdrive policy リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

BitLocker 暗号化の基本ポリシー。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|encryptionMethod|[bitlockerencryptionmethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|オペレーティングシステムドライブの暗号化方法を選択します。 使用可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。|
|startupAuthenticationRequired|Boolean|起動時に追加の認証を要求します。|
|startupAuthenticationBlockWithoutTpmChip|Boolean|互換性のある TPM を使用せずに BitLocker を許可するかどうかを示します (パスワードまたは USB フラッシュドライブのスタートアップキーが必要です)。|
|startupAuthenticationTpmUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|TPM のスタートアップが許可されているかどうか、または要求/禁止を示します。 可能な値は `blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmPinUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップ pin が許可されているかどうか、または許可/禁止を示します。 可能な値は `blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmKeyUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップキーが許可されているかどうか、または必要/不許可かを示します。 可能な値は `blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmPinAndKeyUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップ pin キーとキーが許可されているかどうか、または許可/不許可かを示します。 可能な値は `blocked`、`required`、`allowed` です。|
|minimumPinLength|Int32|スタートアップ pin の最小の長さを示します。 有効な値は4から20までです|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|必要なスタートアップキー情報がない場合に BitLocker で暗号化されたオペレーティングシステムドライブを回復できるようにします。 このポリシー設定は、BitLocker を有効にしたときに適用されます。|
|prebootRecoveryEnableMessageAndUrl|Boolean|ブート前の回復メッセージと Url を有効にします。 requirestartupauthentication が false の場合、この値は影響を与えません。|
|prebootrecoverymessage|String|カスタムの回復メッセージを定義します。|
|prebootrecoveryurl|String|カスタムの回復 URL を定義します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```




