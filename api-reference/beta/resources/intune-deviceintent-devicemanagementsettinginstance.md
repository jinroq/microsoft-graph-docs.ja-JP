---
title: deviceManagementSettingInstance リソースの種類
description: 設定インスタンスの基本型
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 628ca393006666f7a655cf45832784e88f2a4d01
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984493"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>deviceManagementSettingInstance リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定インスタンスの基本型

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementSettingInstances を一覧表示する](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementSettingInstance を取得する](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|設定インスタンス ID|
|definitionId|String|このインスタンスの設定定義の ID|
|valueJson|String|値の JSON 表現|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```





