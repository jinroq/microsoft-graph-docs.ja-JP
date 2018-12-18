---
title: bitLockerRecoveryOptions リソースの種類
description: BitLocker の回復オプションです。
author: tfitzmac
ms.openlocfilehash: c85ce3111ed88ce8e8bf54c98d5fd3122571a0be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310606"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitLockerRecoveryOptions リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

BitLocker の回復オプションです。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|blockDataRecoveryAgent|ブール型|回復エージェントの証明書ベースのデータをブロックするかどうかを示します。|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|ユーザーの許可または固定の 48 桁の回復パスワードを生成するために必要なのかどうか、またはシステム ディスクを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|ユーザーの許可または固定の 256 ビットの回復キーを生成するために必要なのかどうか、またはシステム ディスクを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|hideRecoveryOptions|ブール型|固定の BitLocker セットアップ ウィザードの回復オプションを表示できるようにするかどうか、またはシステム ディスクを示します。|
|enableRecoveryInformationSaveToStore|ブール型|AD DS に格納するのには BitLocker 回復情報を許可するかどうかを示します。|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|どのようなさまざまな BitLocker 回復情報が AD DS に格納されている構成です。 使用可能な値は、`passwordAndKey`、`passwordOnly` です。|
|enableBitLockerAfterRecoveryInformationToStore|ブール型|AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```





