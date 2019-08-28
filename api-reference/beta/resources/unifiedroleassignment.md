---
title: unifiedRoleAssignment リソースの種類
description: 役割の割り当ては、アクセスを許可することを目的とした、特定のスコープのロール定義とプリンシパル間のリンクです。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cfc0c00add243b98c852a00f0a4ab990c3ca5173
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437791"
---
# <a name="unifiedroleassignment-resource-type"></a>unifiedRoleAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleAssignment は、リソースへのアクセスを許可するために使用されます。 これは、特定の範囲のプリンシパル (通常はユーザー) に割り当てられたロール定義を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [UnifiedRoleAssignment を取得する](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | UnifiedRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [UnifiedRoleAssignment を作成する](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | RoleAssignment コレクションへの投稿によって新しい unifiedRoleAssignment を作成します。 |
| [Delete](../api/unifiedroleassignment-delete.md) | None | UnifiedRoleAssignment オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|id|String| UnifiedRoleAssignment の一意識別子。 キー。 null 許容ではありません。読み取り専用です。 |
|principalId|String| 割り当てが付与されるプリンシパルの Objectid。 |
|resourceScope|String| UnifiedRoleAssignment が適用される範囲。 これは、サービス全体の場合は "/" です。 |
|roleDefinitionId|String| 割り当ての対象となる unifiedRoleDefinition。 読み取り専用です。 |

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
