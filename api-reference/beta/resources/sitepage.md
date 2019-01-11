---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.openlocfilehash: d4673138106e23afedb5ff0f28d8ce72fa2797b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871492"
---
# <a name="sitepage-resource"></a>sitePage リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

このリソースは、サイト ページの[一覧][]でページを表します。
タイトル、レイアウト、および[web パーツ][]の s のコレクションが含まれています。

## <a name="tasks-on-a-page"></a>ページ上のタスク

**SitePage**リソースの次のタスクを利用できます。
以下のすべての例は、[サイト][]では、例えば: `https://graph.microsoft.com/{api-version}/sites/{site-id}`。

| 共通タスク                     | HTTP メソッド
|:--------------------------------|:------------------------------
| [List pages][]                  | /Pages を取得します。
| [Get page][]                    | /Pages/{ページの id を取得します。
| [Create][]                      | 投稿/pages
| [Delete][]                      | /Pages/{ページの id を削除します。
| [Publish][]                     | /Pages/{ページ id} の投稿し、公開

[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>JSON 表記

ここでは、 **sitePage**リソースの JSON 表現です。

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

**SitePage**リソースでは、次のプロパティがあります。

| プロパティ名    | Type                         | 説明
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | ページのコンテンツの種類です。

## <a name="page-content"></a>ページのコンテンツ

**SitePage**リソースでは、次のコンテンツのフィールドがあります。

| プロパティ名      | Type                       | 説明
|:-------------------|:---------------------------|:---------------------------
| タイトル              | 文字列                     | ページのタイトル。
| pageLayout         | 文字列                     | ページのページ レイアウトの名前。
| web パーツ           | [web パーツ][]                | ページ上の web パーツです。

## <a name="authoring-metadata"></a>メタデータを作成する

**SitePage**のリソースには、次の作成に関連するメタデータがあります。 PublishingState プロパティは、このようなチェック アウトされているか、公開の状態を作成するページに反映されます。

| プロパティ名          | Type                   | 説明
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | 発行のステータスと MM.mm バージョンのページです。

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | Type              | 説明
|:---------------------|:------------------|:----------------------------------
| ID                   | 文字列            | アイテムの一意識別子。読み取り専用です。
| name                 | 文字列            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| eTag                 | 文字列            | アイテムの ETag。読み取り専用です。
| lastModifiedBy       | [identitySet][]   | このアイテムの最終変更者の ID です。 読み取り専用です。
| lastModifiedDateTime | DateTimeOffset    | アイテムが最後に変更された日時。読み取り専用です。
| parentReference      | [itemReference][] | アイテムが最後に変更された日時。読み取り専用です。
| webUrl               | string (URL)      | ブラウザーでアイテムを表示する URL。読み取り専用です。

## <a name="relationships"></a>リレーションシップ

**SitePage**リソースには、他のリソースへのリレーションシップがありません。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[リスト]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[web パーツ]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
