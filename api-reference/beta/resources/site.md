---
author: JeremyKelley
description: サイト リソースは、SharePoint サイトのメタデータとリレーションシップを提供します。
ms.date: 09/10/2017
title: サイト
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 691f91b63fdff583476c5308f4b8370a563120a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008356"
---
# <a name="site-resource-type"></a>サイトのリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**サイト** リソースは、SharePoint サイトのメタデータとリレーションシップを提供します。

## <a name="methods"></a>メソッド

| Method                         | REST パス
|:-------------------------------|:--------------------------------------------
| [ルート サイトを取得する][]              | GET /sites/root
| [サイトを取得する][]                   | GET /sites/{site-id}
| [パスを使用してサイトを取得する][]           | GET /sites/{hostname}:/{site-path}
| [グループのサイトを取得する][]       | GET /groups/{group-id}/sites/root
| [分析を取得する][]              | GET /sites/{site-id}/analytics
| [間隔によりアクティビティを取得する][] | GET /sites/{site-id}/getActivitiesByInterval
| [ページを一覧表示する][]                 | GET /sites/{site-id}/pages
| [ルート サイトを一覧表示する][]            | GET /sites?filter=root ne null&select=siteCollection,webUrl
| [サイトを検索する][]           | GET /sites?search={query}
| [サイトをフォローする][]                | POST /users/{user-id}/followedSites/add
| [サイトのフォローを取り消す][]              | POST /users/{user-id}/followedSites/remove

[サイトを取得する]: ../api/site-get.md
[ルート サイトを取得する]: ../api/site-get.md
[パスを使用してサイトを取得する]: ../api/site-getbypath.md
[グループのサイトを取得する]: ../api/site-get.md
[分析を取得する]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivity-getbyinterval.md
[ページを一覧表示する]: ../api/sitepage-list.md
[ルート サイトを一覧表示する]: ../api/site-list.md
[サイトを検索する]: ../api/site-search.md
[サイトをフォローする]: ../api/site-follow.md
[サイトのフォローを取り消す]: ../api/site-unfollow.md


## <a name="properties"></a>プロパティ

| プロパティ名            | 種類               | 説明
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | 文字列             | アイテムの[一意識別子](#id-property)。 読み取り専用です。
| **createdDateTime**      | DateTimeOffset     | アイテムが作成された日時。読み取り専用です。
| **説明**          | string             | サイトの説明テキスト。
| **eTag**                 | string             | アイテムの ETag。読み取り専用です。                                                                  |
| **displayName**          | string             | サイトの完全なタイトル。読み取り専用です。
| **lastModifiedDateTime** | DateTimeOffset     | アイテムが最後に変更された日時。読み取り専用です。
| **name**                 | string             | アイテムの名前/タイトル。
| **root**                 | [root][]           | 存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。
| **sharepointIds**        | [sharepointIds][]  | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。
| **siteCollection**       | [siteCollection][] | サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。
| **webUrl**               | string (URL)       | ブラウザーでアイテムを表示する URL。読み取り専用です。

### <a name="id-property"></a>ID プロパティ
**サイト**は、次の値の複合である一意な ID によって識別されます。
* サイト コレクションのホスト名 (contoso.sharepoint.com)
* サイト コレクションの一意 ID (GUID)
* サイトの一意 ID (GUID)
  
`root` 識別子は次に示すように、常にターゲットのルート サイトを参照します。

* `/sites/root`:テナントのルート サイト。
* `/groups/{group-id}/sites/root`:グループのチーム サイト。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                             | 説明
|:------------------|:---------------------------------|:----------------------
| **analytics**     | [itemAnalytics][] リソース       | このサイトで行われたビュー アクティビティに関する分析。
| **列**       | Collection([columnDefinition][]) | このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。
| **contentTypes**  | Collection([contentType][])      | このサイトに定義されたコンテンツ タイプのコレクションです。
| **drive**         | [ドライブ][]                        | このサイトの既定ドライブ (ドキュメント ライブラリ)。
| **ドライブ**        | Collection([drive][])            | このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。
| **アイテム**         | Collection([baseItem][])         | このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。
| **lists**         | Collection([list][])             | このサイトにあるリストのコレクションです。
| **pages**         | Collection([sitePage][])         | このサイトにある SitePages リストのページのコレクション。
| **sites**         | Collection([サイト][])             | このサイトの下のサブサイトのコレクション。

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a>JSON 表記

以下は、**サイト** リソースの JSON 表記です。

**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->
