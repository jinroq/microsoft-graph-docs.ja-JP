---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 609d4202069f6e4258c9824a65b72ab769c365b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981855"
---
# <a name="rolescopetag-resource-type"></a>roleScopeTag リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|ID|String|エンティティのキー。 これは読み取り専用で、自動生成されます。|
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





