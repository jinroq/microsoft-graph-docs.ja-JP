---
title: bitlockerrecoveryoptions リソースの種類
description: BitLocker 回復オプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8bbf0db0ca6dd784a47d1bfb5d743ae17695b81
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142113"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitlockerrecoveryoptions リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

BitLocker 回復オプション。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|blockDataRecoveryAgent|ブール値|証明書ベースのデータ回復エージェントをブロックするかどうかを示します。|
|回復した ypasswordusage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|ユーザーが固定またはシステムディスク用に48桁の回復パスワードを生成することを許可または要求するかどうかを示します。 可能な値は `blocked`、`required`、`allowed` です。|
|recoverykeyusage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|ユーザーが固定またはシステムディスクの256ビット回復キーを生成することを許可または要求するかどうかを示します。 可能な値は `blocked`、`required`、`allowed` です。|
|hideRecoveryOptions|ブール値|固定またはシステムディスクの BitLocker セットアップウィザードでの復元オプションの表示を許可するかどうかを示します。|
|enableRecoveryInformationSaveToStore|ブール値|AD DS に BitLocker 回復情報を格納することを許可するかどうかを示します。|
|recoveryinformationtostore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|AD DS に格納される BitLocker 回復情報の種類を構成します。 使用可能な値は、`passwordAndKey`、`passwordOnly` です。|
|enablebitlockerafterrecoveryinformationtostore|ブール値|AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。|

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




