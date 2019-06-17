---
title: Devicemanagement整数 Settinginstance リソースの種類
description: 整数値を表す設定インスタンス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6f3521eb763062ef9675cb5853562f31049afea
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964040"
---
# <a name="devicemanagementintegersettinginstance-resource-type"></a>Devicemanagement整数 Settinginstance リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

整数値を表す設定インスタンス


[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Devicemanagement整数の Settinginstances を一覧表示する](../api/intune-deviceintent-devicemanagementintegersettinginstance-list.md)|[Devicemanagement整数 Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)コレクション|[Devicemanagement整数 Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[Devicemanagement整数 Settinginstance を取得する](../api/intune-deviceintent-devicemanagementintegersettinginstance-get.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|[Devicemanagement整数 Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Devicemanagement整数 Settinginstance の作成](../api/intune-deviceintent-devicemanagementintegersettinginstance-create.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|新しい[Devicemanagement整数 Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトを作成します。|
|[Devicemanagement整数 Settinginstance の削除](../api/intune-deviceintent-devicemanagementintegersettinginstance-delete.md)|None|[Devicemanagement整数の Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)を削除します。|
|[Devicemanagement整数 Settinginstance の更新](../api/intune-deviceintent-devicemanagementintegersettinginstance-update.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|[Devicemanagement整数 Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID|
|definitionId|String|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID|
|valueJson|String|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現|
|値|Int32|整数型 (integer) の値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntegerSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": 1024
}
```





