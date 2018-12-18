---
title: bitLockerSystemDrivePolicy リソースの種類
description: BitLocker 暗号化の基本ポリシーです。
author: tfitzmac
ms.openlocfilehash: ba1199970099bb841fc363a747abb5b8dcac2ec1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332285"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>bitLockerSystemDrivePolicy リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

BitLocker 暗号化の基本ポリシーです。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|オペレーティング システム ドライブの暗号化方法を選択します。 可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。|
|startupAuthenticationRequired|ブール型|起動時に追加の認証が必要です。|
|startupAuthenticationBlockWithoutTpmChip|ブール型|なし (または USB フラッシュ ドライブにスタートアップ キーのパスワードが必要です)、互換性のある TPM は BitLocker を許可するかどうかを示します。|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップを許可または必要と許可しないかどうかを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップの暗証番号 (pin) を許可または必要と許可しないかどうかを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|スタートアップ キーを TPM を許可または必要と許可しないかどうかを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|TPM スタートアップに追加することを示しますキーとキーは、許可または必要と許可しません。 可能な値は、`blocked`、`required`、`allowed` です。|
|minimumPinLength|Int32|スタートアップの暗証番号 (pin) の最小の長さを示します。 4 ~ 20 の有効な値|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|必要なスタートアップ キー情報がない場合、BitLocker で暗号化されたオペレーティング システム ドライブを回復することができます。 BitLocker を有効にするときは、このポリシー設定が適用されます。|
|prebootRecoveryEnableMessageAndUrl|ブール型|ブート前の回復のメッセージと Url を有効にします。 RequireStartupAuthentication が false の場合、この値は影響しません。|
|prebootRecoveryMessage|String|回復のカスタム メッセージを定義します。|
|prebootRecoveryUrl|String|回復のカスタム URL を定義します。|

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





