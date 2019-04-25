---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 82a14f6462604b732119b90d037b2fab711df5af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507841"
---
# <a name="drive-resource-type"></a>Drive リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。

OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。

## <a name="json-representation"></a>JSON 表記

Drive リソースの JSON 表記を以下に示します。

**drive** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ             | 型                          | 説明                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | アイテム作成の日時。読み取り専用です。                                                                                                                                                                                       |
| 説明          | String                        | ユーザーに表示されるドライブの説明を提供します。 読み取り/書き込み。
| driveType            | String                        | このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。 |
| id                   | String                        | ドライブの一意識別子。読み取り専用。                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | アイテムが最後に変更された日時。読み取り専用です。                                                                                                                                                                             |
| name                 | string                        | アイテムの名前。読み取り/書き込み。                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | 省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。                                                                                                                                                                       |
| quota                | [quota](quota.md)             | 省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。                                                                                                                                                         |
| system               | [systemFacet][]               | 存在する場合は、これがシステム管理のドライブであることを示しています。 読み取り専用です。
| webUrl               | string (URL)                  | ブラウザーでリソースを表示するための URL。読み取り専用です。                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                                 | 説明
|:-------------|:-------------------------------------|:-----------------------
| アクティビティ   | [itemActivity][] コレクション          | このドライブに対して行われた最近のアクティビティのリストです。
| items        | [driveitem](driveitem.md) コレクション | ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。
| root         | [driveitem](driveitem.md)            | ドライブのルート フォルダー。読み取り専用。
| special      | [driveitem](driveitem.md) コレクション | OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。
| フォロー中    | [DriveItem](driveitem.md) コレクション | ユーザーがフォローしているアイテムの一覧。 OneDrive for Business のみ。

## <a name="methods"></a>メソッド

|                        共通タスク                         |         HTTP メソッド         |
| :--------------------------------------------------------- | :-------------------------- |
| [別の Drive の Drive メタデータを取得する][drive-get]           | `GET /drives/{drive-id}`    |
| [ユーザーの既定のドライブのルート フォルダーを取得する][item-get]       | `GET /drive/root`           |
| [ドライブのアクティビティを一覧表示する][drive-activities]        | `GET /drive/activities`     |
| [フォローされたアイテムを一覧表示する][drive-following]                     | `GET /drive/following`      |
| [ドライブの子を一覧表示する][item-children]             | `GET /drive/root/children`  |
| [ドライブ内のすべてのアイテムの変更を一覧表示する][item-changes]    | `GET /drive/root/delta`     |
| [ドライブ内のアイテムを検索する][item-search]               | `GET /drive/root/search`    |
| [特別なフォルダーにアクセスする](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

前の表では例に `/drive` を使用していますが、他のパスも有効です。

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
