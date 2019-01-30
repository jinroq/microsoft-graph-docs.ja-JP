---
title: DriveItemVersion リソースの種類
description: '**DriveItemVersion**リソースは、DriveItem の特定のバージョンを表します。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643987"
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
| [バージョンの復元][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

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

|      プロパティ名       |                         型                         |                               説明                               |
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
