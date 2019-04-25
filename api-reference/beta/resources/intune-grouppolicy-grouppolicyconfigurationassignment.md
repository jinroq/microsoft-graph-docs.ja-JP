---
title: grouppolicyconfigurationassignment リソースの種類
description: グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6fcd7ace912075189ec3e9b5a817181dd392a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575822"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>grouppolicyconfigurationassignment リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicyconfigurationassignments のリスト](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicyconfigurationassignment の取得](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicyconfigurationassignment の作成](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|新しい[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。|
|[grouppolicyconfigurationassignment の削除](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|なし|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。|
|[grouppolicyconfigurationassignment の更新](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|グループポリシー構成を対象としたグループの種類。|

## <a name="relationships"></a>関係
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





