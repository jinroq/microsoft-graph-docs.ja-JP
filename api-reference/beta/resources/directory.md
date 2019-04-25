---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22c5b959f87b6178fa406bc4fd5d00ad52e5cf55
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535244"
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

## <a name="properties"></a>プロパティ
| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|id|String| オブジェクトの一意識別子 (例: 12345678-9abc-def0-1234-56789abcde)。 キー。 null 許容ではありません。 読み取り専用です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|deleteditems|[directoryObject](directoryobject.md) コレクション| 最近削除されたアイテム 読み取り専用。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/directory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
