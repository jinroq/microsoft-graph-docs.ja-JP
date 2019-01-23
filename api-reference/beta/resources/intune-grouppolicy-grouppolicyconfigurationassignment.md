---
title: groupPolicyConfigurationAssignment リソースの種類
description: グループ ポリシー設定の割り当てエンティティでは、特定のグループ ポリシーの構成を AAD の 1 つまたは複数のグループが割り当てられます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 508581ba7b5ac689338c179f4f6b211928c9abaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430333"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>groupPolicyConfigurationAssignment リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループ ポリシー設定の割り当てエンティティでは、特定のグループ ポリシーの構成を AAD の 1 つまたは複数のグループが割り当てられます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyConfigurationAssignments](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション|[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyConfigurationAssignment を取得します。](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyConfigurationAssignment を作成します。](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|新しい[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。|
|[GroupPolicyConfigurationAssignment を削除します。](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|なし|の[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。|
|[GroupPolicyConfigurationAssignment を更新します。](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|グループの種類は、グループ ポリシーの構成を対象とします。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




