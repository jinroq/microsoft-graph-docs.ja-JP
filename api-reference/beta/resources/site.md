---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.openlocfilehash: fb91e9bada227f1a22cf862726ea0b6f658fe469
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871023"
---
# <a name="site-resource-type"></a>サイト リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。

## <a name="methods"></a>メソッド

| Method                         | REST パス
|:-------------------------------|:--------------------------------------------
| [ルート サイトを取得する][]              | GET /sites/root
| [サイトを取得する][]                   | GET /sites/{site-id}
| [パスを使用してサイトを取得する][]           | GET /sites/{hostname}:/{site-path}
| [グループのサイトを取得する][]       | GET /groups/{group-id}/sites/root
| [分析を取得します。][]              | GET/sites/{サイト id}/分析
| [間隔によってアクティビティを取得します。][] | GET/sites/{サイト id}/getActivitiesByInterval
| [List pages][]                 | GET/sites/{サイト id} ページ/
| [ルート サイトの一覧][]            | GET/sites ですか? フィルター = null と選択のルート ne = siteCollection、webUrl
| [サイトを検索する][]           | GET /sites?search={query}

[サイトを取得する]: ../api/site-get.md
[ルート サイトを取得する]: ../api/site-get.md
[パスを使用してサイトを取得する]: ../api/site-getbypath.md
[グループのサイトを取得する]: ../api/site-get.md
[分析を取得します。]: ../api/itemanalytics-get.md
[間隔によってアクティビティを取得します。]: ../api/itemactivity-getbyinterval.md
[List pages]: ../api/sitepage-list.md
[ルート サイトの一覧]: ../api/site-list.md
[サイトを検索する]: ../api/site-search.md


## <a name="properties"></a>プロパティ

| プロパティ名            | Type               | 説明
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | string             | アイテムの一意識別子。読み取り専用です。
| **createdDateTime**      | DateTimeOffset     | アイテムが作成された日時。読み取り専用です。
| **説明**          | 文字列             | サイトの説明テキスト。
| **eTag**                 | 文字列             | アイテムの ETag。読み取り専用です。                                                                  |
| **displayName**          | 文字列             | サイトの完全なタイトル。読み取り専用です。
| **lastModifiedDateTime** | DateTimeOffset     | アイテムが最後に変更された日時。読み取り専用です。
| **name**                 | 文字列             | アイテムの名前/タイトル。
| **root**                 | [root][]           | 存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。
| **sharepointIds**        | [sharepointIds][]  | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。
| **siteCollection**       | [siteCollection][] | サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。
| **webUrl**               | string (URL)       | ブラウザーでアイテムを表示する URL。読み取り専用です。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                             | 説明
|:------------------|:---------------------------------|:----------------------
| **分析**     | [itemAnalytics][]リソース       | このサイトで行われた活動の表示について分析します。
| **columns**       | Collection([columnDefinition][]) | このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。
| **contentTypes**  | Collection([contentType][])      | このサイトに定義されたコンテンツ タイプのコレクションです。
| **drive**         | [ドライブ][]                        | このサイトの既定ドライブ (ドキュメント ライブラリ)。
| **ドライブ**        | Collection([drive][])            | このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。
| **アイテム**         | Collection([baseItem][])         | このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。
| **lists**         | Collection([list][])             | このサイトにあるリストのコレクションです。
| **ページ**         | コレクション ([sitePage][])         | このサイトのサイト ページのリスト内のページのコレクションです。
| **sites**         | Collection([サイト][])             | このサイトの下のサブサイトのコレクション。

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[ドライブ]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[リスト]: list.md
[sitePage]: sitepage.md
[ルート]: root.md
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
