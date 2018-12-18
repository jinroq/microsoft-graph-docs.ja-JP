---
title: bitLockerFixedDrivePolicy リソースの種類
description: BitLocker は、ドライブのポリシーを修正します。
author: tfitzmac
ms.openlocfilehash: 71fc28fc88689165cdcd187542460432948f78c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342617"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a>bitLockerFixedDrivePolicy リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

BitLocker は、ドライブのポリシーを修正します。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|固定のドライブの暗号化方法を選択します。 可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。|
|requireEncryptionForWriteAccess|Boolean|このポリシー設定は、BitLocker の保護が固定データ ドライブをコンピューターに書き込み可能にするために必要かどうかを判断します。|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|このポリシー設定では、BitLocker で保護された方法固定データ ドライブは、必要な資格情報がない場合にリカバリを制御できます。 BitLocker を有効にするときは、このポリシー設定が適用されます。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```





