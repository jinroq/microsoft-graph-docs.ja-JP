---
title: deviceManagementScriptGroupAssignment リソースの種類
description: グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11e4093c1a92f13b71cf205e48db1a7b8a5c444f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942053"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>deviceManagementScriptGroupAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementScriptGroupAssignments の一覧を表示する](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementScriptGroupAssignment の取得](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementScriptGroupAssignment の作成](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|新しい[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。|
|[DeviceManagementScriptGroupAssignment の削除](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|None|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を削除します。|
|[DeviceManagementScriptGroupAssignment の更新](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[デバイス管理スクリプト] グループ割り当てエンティティのキー。|
|targetGroupId|String|スクリプトを対象としている Azure Active Directory グループの Id。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




