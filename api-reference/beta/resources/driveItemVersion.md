---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3be7cd044b65eccd2370a2848258b415c5e70b00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543219"
---
# <a name="driveitemversion-resource-type"></a>DriveItemVersion リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>プロパティ

|      プロパティ名       |                         種類                         |                               説明                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | バージョンの ID。 読み取り専用。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 最後にバージョンを変更したユーザーの ID。 読み取り専用です。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | バージョンが最後に変更された日時。 読み取り専用。                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | 特定のバージョンのパブリケーション ステータスを示します。 読み取り専用です。 |
| **size**                 | Int64                                                | アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。  |

## <a name="relationships"></a>リレーションシップ

次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。

| リレーションシップ名 |  種類  |            説明             |
| :---------------- | :----- | :--------------------------------- |
| **content**       | ストリーム | バージョンのコンテンツ ストリーム。 |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/driveItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
