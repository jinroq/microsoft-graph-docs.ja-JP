---
title: deviceManagementStringSettingInstance リソースの種類
description: 文字列値を表す設定インスタンス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f29113a104dba8b27ccdacd25286467fe6b725bb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943313"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a>deviceManagementStringSettingInstance リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

文字列値を表す設定インスタンス


[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementStringSettingInstances を一覧表示する](../api/intune-deviceintent-devicemanagementstringsettinginstance-list.md)|[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)コレクション|[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementStringSettingInstance を取得する](../api/intune-deviceintent-devicemanagementstringsettinginstance-get.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementStringSettingInstance の作成](../api/intune-deviceintent-devicemanagementstringsettinginstance-create.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|新しい[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトを作成します。|
|[DeviceManagementStringSettingInstance の削除](../api/intune-deviceintent-devicemanagementstringsettinginstance-delete.md)|None|[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)を削除します。|
|[DeviceManagementStringSettingInstance の更新](../api/intune-deviceintent-devicemanagementstringsettinginstance-update.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID|
|definitionId|String|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID|
|valueJson|String|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現|
|value|文字列型 (String)|文字列型 (string) の値|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementStringSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": "String"
}
```




