---
title: deviceConfigurationGroupAssignment リソースの種類
description: デバイス構成のグループの割り当て。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ed94f08fb33fe4a999e71b85808f58853d40cad4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406823"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a>deviceConfigurationGroupAssignment リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス構成のグループの割り当て。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceConfigurationGroupAssignments](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DeviceConfigurationGroupAssignment を取得します。](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を参照してください。|
|[DeviceConfigurationGroupAssignment を作成します。](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。|
|[DeviceConfigurationGroupAssignment を削除します。](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|なし|の[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を削除します。|
|[DeviceConfigurationGroupAssignment を更新します。](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|targetGroupId|String|AAD グループの Id は、対象としてデバイスを構成します。|
|excludeGroup|Boolean|かどうかをこのグループを除外するようにします。 既定のグループが含まれている必要があること|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceConfiguration|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|ナビゲーション リンクを対象となるデバイスを構成します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```




