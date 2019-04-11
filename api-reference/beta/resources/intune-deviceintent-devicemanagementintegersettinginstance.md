---
title: devicemanagement整数 settinginstance リソースの種類
description: 整数値を表す設定インスタンス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5987e74f4503a2f84e457a8d59d7219d941f600
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771475"
---
# <a name="devicemanagementintegersettinginstance-resource-type"></a>devicemanagement整数 settinginstance リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

整数値を表す設定インスタンス


[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagement整数の settinginstances を一覧表示する](../api/intune-deviceintent-devicemanagementintegersettinginstance-list.md)|[devicemanagement整数 settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)コレクション|[devicemanagement整数 settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagement整数 settinginstance を取得する](../api/intune-deviceintent-devicemanagementintegersettinginstance-get.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|[devicemanagement整数 settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagement整数 settinginstance の作成](../api/intune-deviceintent-devicemanagementintegersettinginstance-create.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|新しい[devicemanagement整数 settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトを作成します。|
|[devicemanagement整数 settinginstance の削除](../api/intune-deviceintent-devicemanagementintegersettinginstance-delete.md)|なし|[devicemanagement整数の settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)を削除します。|
|[devicemanagement整数 settinginstance の更新](../api/intune-deviceintent-devicemanagementintegersettinginstance-update.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|[devicemanagement整数 settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID|
|definitionId|文字列|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID|
|valuejson|文字列|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現|
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





