---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a63ac05ea6161843aa1ad664a99003b7f69d38e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400565"
---
# <a name="rolescopetag-resource-type"></a>roleScopeTag リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ロールのスコープのタグ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を一覧表示します。|
|[RoleScopeTag を取得します。](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティと関係を参照してください。|
|[RoleScopeTag を作成します。](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|新しい[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。|
|[RoleScopeTag を削除します。](../api/intune-rbac-rolescopetag-delete.md)|なし|の[roleScopeTag](../resources/intune-rbac-rolescopetag.md)を削除します。|
|[RoleScopeTag を更新します。](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 これは読み取り専用で、自動生成されます。|
|displayName|String|表示する、またはロールのスコープのタグの表示名。|
|説明|String|ロールのスコープのタグの説明です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```




