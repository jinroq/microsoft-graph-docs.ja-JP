---
title: Bitlockersystemdrive Policy リソースの種類
description: BitLocker 暗号化の基本ポリシー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4ffeaca0d5ee305690c05337eeb75787ece9641
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333766"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>Bitlockersystemdrive Policy リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

BitLocker 暗号化の基本ポリシー。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|オペレーティングシステムドライブの暗号化方法を選択します。 使用可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。|
|startupAuthenticationRequired|Boolean|起動時に追加の認証を要求します。|
|startupAuthenticationBlockWithoutTpmChip|Boolean|互換性のある TPM を使用せずに BitLocker を許可するかどうかを示します (パスワードまたは USB フラッシュドライブのスタートアップキーが必要です)。|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM のスタートアップが許可されているかどうか、または要求/禁止を示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップ pin が許可されているかどうか、または許可/禁止を示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップキーが許可されているかどうか、または必要/不許可かを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップ pin キーとキーが許可されているかどうか、または許可/不許可かを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|minimumPinLength|Int32|スタートアップ pin の最小の長さを示します。 有効な値は4から20までです|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|必要なスタートアップキー情報がない場合に BitLocker で暗号化されたオペレーティングシステムドライブを回復できるようにします。 このポリシー設定は、BitLocker を有効にしたときに適用されます。|
|prebootRecoveryEnableMessageAndUrl|Boolean|ブート前の回復メッセージと Url を有効にします。 RequireStartupAuthentication が false の場合、この値は影響を与えません。|
|prebootRecoveryMessage|String|カスタムの回復メッセージを定義します。|
|prebootRecoveryUrl|String|カスタムの回復 URL を定義します。|

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



