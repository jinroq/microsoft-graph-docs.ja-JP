---
title: DriveItemVersion リソースの種類
description: '**DriveItemVersion**リソースは、DriveItem の特定のバージョンを表します。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b6e9ecd2c3c8ec14958cfa2645f8fb0dbfe30e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949592"
---
# <a name="driveitemversion-resource-type"></a>DriveItemVersion リソースの種類

**DriveItemVersion** リソースは、[DriveItem](driveitem.md) の特定のバージョンを表しています。


## <a name="tasks-on-driveitemversion-resources"></a>DriveItemVersion リソースのタスク

driveItemVersion リソースで使用可能なタスクを次に示します。

|            共通タスク             |         HTTP メソッド         |
| :--------------------------------- | :-------------------------- |
| [バージョンの一覧表示][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [バージョンの取得][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [コンテンツの取得][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [バージョンの復元][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

前の表では、例に `/drive` を使用していますが、他にも有効な要求が多数あります。

## <a name="json-representation"></a>JSON 表記

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a>プロパティ

|      プロパティ名       |                         Type                         |                               説明                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | バージョンの ID。 読み取り専用です。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 最後にバージョンを変更したユーザーの ID。 読み取り専用です。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | バージョンが最後に変更された日時。 読み取り専用です。                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | 特定のバージョンのパブリケーション ステータスを示します。 読み取り専用です。 |
| **size**                 | Int64                                                | アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。  |
| **content**              | ストリーム                                               | 項目のこのバージョンのコンテンツ ストリーム。                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
