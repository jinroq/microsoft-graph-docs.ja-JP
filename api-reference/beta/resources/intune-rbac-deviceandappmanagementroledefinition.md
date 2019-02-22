---
title: deviceAndAppManagementRoleDefinition リソースの種類
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bee2a27e22a44925dfdc9f36a52e0067fbc72cac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139894"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a>deviceAndAppManagementRoleDefinition リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。


[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceAndAppManagementRoleDefinitions のリスト](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) コレクション|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceAndAppManagementRoleDefinition の取得](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceAndAppManagementRoleDefinition の作成](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。|
|[deviceAndAppManagementRoleDefinition の削除](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|なし|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の削除|
|[deviceAndAppManagementRoleDefinition の更新](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 これは読み取り専用で、自動生成されます。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|displayName|String|ロールの定義の表示名。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|説明|String|ロールの定義の説明。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|permissions|[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション|このロールに実行が許可されている、ロールのアクセス許可のリスト。 これらは、rolePermission の一部として定義されている actionName と一致する必要があります。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|rolePermissions|[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション|このロールに実行が許可されている、ロールのアクセス許可のリスト。 これらは、rolePermission の一部として定義されている actionName と一致する必要があります。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|isBuiltInRoleDefinition|Boolean|ロールの種類。 組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|isBuiltIn|Boolean|ロールの種類。 組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション|このロールの定義の、ロールの割り当てのリスト。 [roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




