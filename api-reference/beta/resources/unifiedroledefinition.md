---
title: unifiedRoleDefinition リソースの種類
description: 統合ロール定義は、アクセス許可のコレクションです。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: be1b8a0b1a623c6cf322d5cf7997f04b87875c51
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437749"
---
# <a name="unifiedroledefinition-resource-type"></a>unifiedRoleDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleDefinition は、読み取り、書き込み、削除などの実行可能な操作を一覧表示するアクセス許可のコレクションです。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リスト unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md)コレクション | UnifiedRoleDefinition オブジェクトとそのプロパティのリストを読み取ります。 |
| [UnifiedRoleDefinition を取得する](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | UnifiedRoleDefinition オブジェクトのプロパティを読み取ります。 |
| [UnifiedRoleDefinition を作成する](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | UnifiedRoleDefinition オブジェクトを作成します。 |
| [UnifiedRoleDefinition の更新](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | UnifiedRoleDefinition オブジェクトを更新します。 |
| [UnifiedRoleDefinition の削除](../api/unifiedroledefinition-delete.md) | None | UnifiedRoleDefinition オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|description|String| UnifiedRoleDefinition の説明。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|displayName|String| UnifiedRoleDefinition の表示名。 IsBuiltIn が true の場合は、値の取得のみ可能です。 必須。|
|id|文字列| UnifiedRoleDefinition の一意識別子。 キー。 null 許容ではありません。読み取り専用です。 |
|isBuiltIn|Boolean| UnifiedRoleDefinition が製品に含まれている既定のセットの一部であるか、またはカスタムであるかを示すフラグ。 読み取り専用。 |
|isEnabled|Boolean| 役割が割り当てに対して有効になっているかどうかを示すフラグ。 False の場合、役割は割り当てに使用できません。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|resourceScopes|String コレクション| ロール定義によって付与される範囲のアクセス許可の一覧が適用されます。 現時点では "/" のみがサポートされています。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|rolePermissions|[unifiedRolePermission](unifiedrolepermission.md)コレクション| 役割に含まれるアクセス許可の一覧。 IsBuiltIn が true の場合は、値の取得のみ可能です。 必須です。 |
|templateId|String| IsBuiltIn が false のときに設定できるカスタムテンプレート識別子。 この識別子は、通常、異なるディレクトリ間で識別子を同じにする必要がある場合に使用されます。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|version|String| UnifiedRoleDefinition のバージョンを示します。 IsBuiltIn が true の場合は、値の取得のみ可能です。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
