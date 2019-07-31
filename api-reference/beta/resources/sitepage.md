---
author: rahmit
description: このリソースは、SitePages リストのページを表します。
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240ab50f31d500fad960768bb6c45cb9c6ff6511
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965048"
---
# <a name="sitepage-resource"></a>sitePage リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このリソースは、SitePages[リスト][]のページを表します。
これには、タイトル、レイアウト、および[webPart][]のコレクションが含まれています。

## <a name="tasks-on-a-page"></a>ページ上のタスク

**Sitepage**リソースでは、次のタスクを使用できます。
以下のすべての例は、[サイト][]に関連し`https://graph.microsoft.com/{api-version}/sites/{site-id}`ています。例:。

| 共通タスク                     | HTTP メソッド
|:--------------------------------|:------------------------------
| [ページを一覧表示する][]                  | ページを取得する
| [ページを取得する][]                    | ページを取得する/ページ/{pagefrom id}
| [Create][]                      | 投稿/ページ
| [Delete][]                      | 削除/ページ/{page¥ id}
| [Publish][]                     | 投稿/ページ/_ page/発行

[ページを一覧表示する]: ../api/sitepage-list.md
[ページを取得する]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>JSON 表記

ここでは、 **Sitepage**リソースの JSON 表記を示します。

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

**Sitepage**リソースには、次のプロパティがあります。

| プロパティ名    | 種類                         | 説明
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | ページのコンテンツタイプ。

## <a name="page-content"></a>ページのコンテンツ

**Sitepage**リソースには、次のコンテンツフィールドがあります。

| プロパティ名      | 種類                       | 説明
|:-------------------|:---------------------------|:---------------------------
| title              | string                     | ページのタイトル。
| pageLayout         | string                     | ページのページレイアウトの名前を指定します。
| パーツ           | [パーツ][]                | ページ上の web パーツ。

## <a name="authoring-metadata"></a>メタデータを作成する

**Sitepage**リソースには、次の作成関連のメタデータがあります。 発行状態プロパティは、チェックアウトまたは発行されたページ作成状態を反映します。

| プロパティ名          | 種類                   | 説明
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | ページの発行状態と MM.mm バージョン。

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | 種類              | 説明
|:---------------------|:------------------|:----------------------------------
| id                   | string            | アイテムの一意識別子。読み取り専用です。
| name                 | string            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| eTag                 | string            | アイテムの ETag。読み取り専用です。
| lastModifiedBy       | [identitySet][]   | このアイテムの最終変更者の ID です。 読み取り専用です。
| lastModifiedDateTime | DateTimeOffset    | アイテムが最後に変更された日時。読み取り専用です。
| parentReference      | [itemReference][] | アイテムが最後に変更された日時。読み取り専用です。
| webUrl               | string (URL)      | ブラウザーでアイテムを表示する URL。読み取り専用です。

## <a name="relationships"></a>リレーションシップ

**Sitepage**リソースには、他のリソースとの関係がありません。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[リスト]: site.md
[パーツ]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": []
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
