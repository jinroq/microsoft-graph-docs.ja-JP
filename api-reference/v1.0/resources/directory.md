---
title: directory リソースの種類 (削除済みアイテム)
description: . 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 627ced59fa87a8e950af96173a807da4d500f428
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032747"
---
# <a name="directory-resource-type-deleted-items"></a>directory リソースの種類 (削除済みアイテム)

ディレクトリ内の削除済みアイテムを表します。 アイテムが削除されると、そのアイテムは削除済みアイテムの「コンテナー」に追加されます。 削除されたアイテムは、最大 30 日間、復元可能な状態に維持されます。 30 日が経過すると、アイテムは完全に削除されます。

現在、[削除済みアイテム] 機能は Office 365 の [group](group.md) および [user](users.md) リソースに対してのみサポートされています。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型 | 説明 |
|:---------------|:------------|:------------|
|[削除済みアイテムの取得](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 削除済みアイテムのプロパティを取得します。 |
|[削除済みアイテムの復元](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 最近削除されたアイテムを復元します。 |
|[削除済みアイテムの一覧表示](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) コレクション| 最近削除されたアイテムのリストを取得します。 |
|[アイテムの完全削除](../api/directory-deleteditems-delete.md) | なし | アイテムを完全に削除します。 |
|[ユーザーが所有する削除済みアイテムを一覧表示する](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | ユーザーが所有しているディレクトリアイテムを一覧表示します。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|deletedItems|[directoryObject](directoryobject.md) コレクション| 最近削除されたアイテム 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a>例

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
