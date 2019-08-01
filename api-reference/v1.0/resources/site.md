---
author: JeremyKelley
ms.author: JeremyKelley
title: サイトのリソース
description: サイトのリソースでは、SharePoint サイトのメタデータとリレーションシップを提供します。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 56df3754ab0fc87e839e3eb71db06ea5b05c75e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034175"
---
# <a name="site-resource"></a>サイトのリソース

**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。

## <a name="methods"></a>メソッド

| メソッド                | 戻り値の種類 | 説明
|:-------------------------|:-------------|:----------
| [ルート サイトを取得する][]        | サイト | テナント内のルートの SharePoint サイトにアクセスします。
| [サイトを取得する][]             | サイト | SiteId を使用して SharePoint サイトにアクセスします。
| [パスを使用してサイトを取得する][]     | サイト | 相対パスを使用してルートの SharePoint サイトにアクセスします。
| [グループのサイトを取得する][] | サイト | グループのチーム サイトにアクセスします。
| [分析を取得する][]              | [itemAnalytics][] | このリソースの分析を取得します。 
| [間隔ごとにアクティビティを取得する][] | [itemActivityStat][] | 指定した時間間隔内に**itemActivityStats**のコレクションを取得します。
| [サイトを検索する][]     | サイトのコレクション | 指定したキーワードと一致するサイトを見つけるために SharePoint のテナント全体を検索します。

[サイトを取得する]: ../api/site-get.md
[ルート サイトを取得する]: ../api/site-get.md
[パスを使用してサイトを取得する]: ../api/site-getbypath.md
[グループのサイトを取得する]: ../api/site-get.md
[分析を取得する]: ../api/itemanalytics-get.md
[間隔ごとにアクティビティを取得する]: ../api/itemactivitystat-getactivitybyinterval.md
[サイトを検索する]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md

## <a name="properties"></a>プロパティ

| プロパティ            | 型                                | 説明                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | アイテムの一意識別子。読み取り専用です。                                                  |
| **createdDateTime**      | DateTimeOffset                      | アイテムが作成された日時。読み取り専用です。                                             |
| **説明**          | string                              | サイトの説明テキスト。                                                             |
| **displayName**          | string                              | サイトの完全なタイトル。読み取り専用です。                                                        |
| **eTag**                 | string                              | アイテムの ETag。読み取り専用です。                                                                  |
| **lastModifiedDateTime** | DateTimeOffset                      | アイテムが最後に変更された日時。読み取り専用です。                                       |
| **name**                 | string                              | アイテムの名前/タイトル。                                                                  |
| **root**                 | [root](root.md)                     | 存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。 |
| **webUrl**               | string (URL)                        | ブラウザーでアイテムを表示する URL。読み取り専用です。                                          |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ      | 型                             | 説明
|:------------------|:---------------------------------|:----------------------
| **analytics**     | [itemAnalytics][] リソース       | このサイトで行われたビュー アクティビティに関する分析。
| **列**       | Collection([columnDefinition][]) | このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。
| **contentTypes**  | Collection([contentType][])      | このサイトに定義されたコンテンツ タイプのコレクションです。
| **drive**         | [ドライブ][]                        | このサイトの既定ドライブ (ドキュメント ライブラリ)。
| **ドライブ**        | Collection([drive][])            | このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。
| **アイテム**         | Collection([baseItem][])         | このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。
| **lists**         | Collection([list][])             | このサイトにあるリストのコレクションです。
| **sites**         | Collection([サイト][])             | このサイトの下のサブサイトのコレクション。
| **onenote**       | [onenote][]                      | ノートブック関連の操作のために OneNote サービスを呼び出します。

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[リスト]: list.md
[サイト]: site.md
[onenote]: onenote.md

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

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
