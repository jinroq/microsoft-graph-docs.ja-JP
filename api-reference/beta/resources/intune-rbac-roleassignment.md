---
title: roleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cffebe54ba79d9b013068b9162f9e3a17447b15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566359"
---
# <a name="roleassignment-resource-type"></a>roleAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[roleAssignments のリスト](../api/intune-rbac-roleassignment-list.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション|[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[roleAssignment の取得](../api/intune-rbac-roleassignment-get.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[roleAssignment の作成](../api/intune-rbac-roleassignment-create.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。|
|[roleAssignment の削除](../api/intune-rbac-roleassignment-delete.md)|なし|[roleAssignment](../resources/intune-rbac-roleassignment.md) を削除します。|
|[roleAssignment の更新](../api/intune-rbac-roleassignment-update.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 これは読み取り専用で、自動生成されます。|
|displayName|String|ロール割り当ての表示名またはフレンドリ名。|
|説明|String|ロール割り当ての説明。|
|scopeMembers|String コレクション|役割のスコープ メンバーのセキュリティ グループの ID リスト。  Azure Active Directory の ID。|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|役割の割り当てのスコープの種類を指定します。 既定の種類 ' resourcescope ' では、を割り当てることができます。 ' alldevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。 使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。|
|resourceScopes|String コレクション|役割のスコープ メンバーのセキュリティ グループの ID リスト。  Azure Active Directory の ID です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|この割り当てが含まれる役割の定義。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```





