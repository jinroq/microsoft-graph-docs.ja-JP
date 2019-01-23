---
title: bitLockerRecoveryOptions リソースの種類
description: BitLocker の回復オプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398514"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitLockerRecoveryOptions リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

BitLocker の回復オプションです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean|回復エージェントの証明書ベースのデータをブロックするかどうかを示します。|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|ユーザーの許可または固定の 48 桁の回復パスワードを生成するために必要なのかどうか、またはシステム ディスクを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|ユーザーの許可または固定の 256 ビットの回復キーを生成するために必要なのかどうか、またはシステム ディスクを示します。 可能な値は、`blocked`、`required`、`allowed` です。|
|hideRecoveryOptions|Boolean|固定の BitLocker セットアップ ウィザードの回復オプションを表示できるようにするかどうか、またはシステム ディスクを示します。|
|enableRecoveryInformationSaveToStore|Boolean|AD DS に格納するのには BitLocker 回復情報を許可するかどうかを示します。|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|どのようなさまざまな BitLocker 回復情報が AD DS に格納されている構成です。 使用可能な値は、`passwordAndKey`、`passwordOnly` です。|
|enableBitLockerAfterRecoveryInformationToStore|Boolean|AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。|

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




