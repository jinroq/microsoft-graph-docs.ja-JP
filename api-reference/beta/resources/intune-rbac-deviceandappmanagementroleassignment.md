---
title: deviceAndAppManagementRoleAssignment リソースの種類
description: 役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 115dfbae5bb333bb512db242d3fc1d58dfca74fb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940009"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a>deviceAndAppManagementRoleAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みのロールに適用されます。


[roleAssignment](../resources/intune-rbac-roleassignment.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceAndAppManagementRoleAssignments](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) コレクション|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|新しい [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを作成します。|
|[Delete deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|なし|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) を削除します。|
|[Update deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 これは読み取り専用で、自動生成されます。 [roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します|
|displayName|String|ロール割り当ての表示名またはフレンドリ名。 [roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します|
|description|String|ロール割り当ての説明。 [roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します|
|scopeMembers|String collection|役割のスコープ メンバーのセキュリティ グループの ID リスト。  Azure Active Directory の ID。 [roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|役割の割り当てのスコープの種類を指定します。 既定の種類 ' ResourceScope ' では、を割り当てることができます。 ' AllDevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。 [Roleassignment](../resources/intune-rbac-roleassignment.md)から継承されます。 使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。|
|resourceScopes|String collection|役割のスコープ メンバーのセキュリティ グループの ID リスト。  Azure Active Directory の ID。 [roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します|
|members|String コレクション|ロール メンバーのセキュリティ グループの ID リスト。 Azure Active Directory の ID です。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|対象割り当てが含まれるロール定義。 [roleAssignment](../resources/intune-rbac-roleassignment.md) からの継承|
|roleScopeTags|[ロール Copetag](../resources/intune-rbac-rolescopetag.md)コレクション|役割の割り当てで定義されている役割のスコープタグのセット。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```




