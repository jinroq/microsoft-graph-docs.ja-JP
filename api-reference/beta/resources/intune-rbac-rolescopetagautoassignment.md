---
title: ロール Copetagautoassignment リソースの種類
description: デバイスに適用する役割スコープタグをグループに自動割り当てるためのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a308c91eb2a78c50012c348a19b613335915af47
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369186"
---
# <a name="rolescopetagautoassignment-resource-type"></a>ロール Copetagautoassignment リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスに適用する役割スコープタグをグループに自動割り当てるためのプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ロールの Copetagautoassignments を一覧表示する](../api/intune-rbac-rolescopetagautoassignment-list.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ロールの Copetagautoassignment の取得](../api/intune-rbac-rolescopetagautoassignment-get.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ロールの Copetagautoassignment の作成](../api/intune-rbac-rolescopetagautoassignment-create.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)|新しい[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトを作成します。|
|[ロール Copetagautoassignment の削除](../api/intune-rbac-rolescopetagautoassignment-delete.md)|None|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)を削除します。|
|[ロールの Copetagautoassignment の更新](../api/intune-rbac-rolescopetagautoassignment-update.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|特定の役割スコープタグの自動割り当てターゲット。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



