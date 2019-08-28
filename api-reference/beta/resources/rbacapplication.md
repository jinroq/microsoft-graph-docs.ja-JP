---
title: rbacApplication リソースの種類
description: Role management ナビゲーションプロパティ
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: afcef3766e4df80a3856ab59684ba826c3a78d14
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437826"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 365 RBAC プロバイダの統合されたロール定義および役割の割り当ての役割管理コンテナー。 サポートされている唯一の RBAC アプリケーションは、現在 "ディレクトリ" です。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [UnifiedRoleAssignment を作成する](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | RoleAssignments コレクションへの投稿によって新しい unifiedRoleAssignment を作成します。 |
| [roleAssignments のリスト](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md)コレクション | UnifiedRoleAssignment オブジェクトのコレクションを取得します。 UnifiedRoleDefitionId または principalId でフィルター処理することで、特定のインスタンスのみを照会できます。 |
| [UnifiedRoleDefinition を作成する](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | RoleDefinitions コレクションへの投稿によって新しい unifiedRoleDefinition を作成します。 |
| [List roleDefinition](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md)コレクション | UnifiedRoleDefinition オブジェクトのコレクションを取得します。 |

## <a name="properties"></a>プロパティ

なし

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

None

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
