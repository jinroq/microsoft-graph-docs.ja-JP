---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b35c2c56c7033cd668b311c17169f5c719e5948
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062083"
---
# <a name="directory-resource-type-deleted-items"></a>directory リソースの種類 (削除済みアイテム)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリ内の削除済みアイテムを表します。 アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。

現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型 | 説明 |
|:---------------|:------------|:------------|
|[削除済みアイテムの取得](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 削除済みアイテムのプロパティを取得します。 |
|[削除済みアイテムの復元](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 最近削除されたアイテムを復元します。 |
|[削除済みアイテムの一覧表示](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) collection| 最近削除されたアイテムのリストを取得します。 |
|[アイテムの完全削除](../api/directory-deleteditems-delete.md) | なし | アイテムを完全に削除します。 |
|[ユーザーが所有する削除済みアイテムを一覧表示する](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | ユーザーが所有しているディレクトリアイテムを一覧表示します。 |
|[リスト featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md)コレクション | FeatureRolloutPolicy オブジェクトのリストを取得します。 |
|[FeatureRolloutPolicy を作成する](../api/directory-post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 新しい featureRolloutPolicy オブジェクトを作成します。 |
| [FeatureRolloutPolicy を取得する](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Featurerolloutpolicy オブジェクトのプロパティとリレーションシップを取得します。 |
| [FeatureRolloutPolicy の更新](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Featurerolloutpolicy オブジェクトのプロパティを更新します。 |
| [FeatureRolloutPolicy の削除](../api/featurerolloutpolicy-delete.md) | None | FeatureRolloutPolicy オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|id|String| オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。 キー。 null 許容ではありません。 読み取り専用です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|deleteditems|[directoryObject](directoryobject.md) コレクション| 最近削除されたアイテム 読み取り専用。 Null 許容型。|
|featureRolloutPolicies|[featureRolloutPolicy](featurerolloutpolicy.md)コレクション| Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
