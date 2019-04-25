---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fb4f0a782d9502f9e3da3f0a7da2389e937a7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573418"
---
# <a name="deviceconfigurationassignment-resource-type"></a>deviceConfigurationAssignment リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceConfigurationAssignments のリスト](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceConfigurationAssignment の取得](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceConfigurationAssignment の作成](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。|
|[deviceConfigurationAssignment の削除](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|なし|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。|
|[deviceConfigurationAssignment の更新](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|割り当てのキー。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|デバイス構成の割り当て先です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



