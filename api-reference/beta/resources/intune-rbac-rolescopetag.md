---
title: roleScopeTag リソースの種類
description: ロールのスコープのタグ
author: tfitzmac
ms.openlocfilehash: 49059ceddcd043f39f51c563c85ba8986b6fc61b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354769"
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

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
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





