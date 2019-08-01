---
title: ListItemVersion リソースの種類
description: '**listItemVersion** リソースは、ListItem リソースの旧バージョンを表しています。'
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 8523e77fd308ab4863a0c3d90ccacad73cc766cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036450"
---
# <a name="listitemversion-resource-type"></a>ListItemVersion リソースの種類

**listItemVersion** リソースは、[ListItem](listitem.md) リソースの旧バージョンを表しています。

## <a name="tasks-on-listitemversion-resources"></a>ListItemVersion リソースのタスク

listItemVersion リソースで使用可能なタスクを次に示します。

|            共通タスク             |         HTTP メソッド         |
| :--------------------------------- | :-------------------------- |
| [バージョンを一覧表示する][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [バージョンの取得][version-get]         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| [バージョンの復元][version-restore] | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>JSON 表記

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>プロパティ

|      プロパティ名       |                         種類                         |                               説明                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | バージョンの ID。 読み取り専用です。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 最後にバージョンを変更したユーザーの ID。 読み取り専用。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | バージョンが最後に変更された日時。 読み取り専用です。                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | 特定のバージョンのパブリケーション ステータスを示します。 読み取り専用です。 |


## <a name="relationships"></a>関係

次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。

| リレーションシップ名 |                      種類                      |                               説明                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**        | [FieldValueSet](../resources/fieldvalueset.md) | このバージョンのリスト アイテムの、フィールドと値のコレクション。 |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
