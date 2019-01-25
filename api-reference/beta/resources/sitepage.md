---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522302"
---
# <a name="sitepage-resource"></a>sitePage リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このリソースは、サイト ページの[一覧][]でページを表します。
タイトル、レイアウト、および[web パーツ][]の s のコレクションが含まれています。

## <a name="tasks-on-a-page"></a>ページ上のタスク

**SitePage**リソースの次のタスクを利用できます。
以下のすべての例は、[][] などのサイトからの相対指定です。

| 共通タスク                     | HTTP メソッド
|:--------------------------------|:------------------------------
| [List pages][]                  | ページを取得する
| [Get page][]                    | /Pages/{ページの id を取得します。
| [Create][]                      | POST pages
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

| プロパティ名    | 型                         | 説明
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | ページのコンテンツの種類です。

## <a name="page-content"></a>ページ コンテンツ

**SitePage**リソースでは、次のコンテンツのフィールドがあります。

| プロパティ名      | 型                       | 説明
|:-------------------|:---------------------------|:---------------------------
| タイトル              | 文字列                     | ページのタイトル。
| pageLayout         | string                     | ページのページ レイアウトの名前。
| web パーツ           | webpart                | ページ上の web パーツです。

## <a name="authoring-metadata"></a>メタデータを作成する

**SitePage**のリソースには、次の作成に関連するメタデータがあります。 PublishingState プロパティは、このようなチェック アウトされているか、公開の状態を作成するページに反映されます。

| プロパティ名          | 型                   | 説明
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | 発行のステータスと MM.mm バージョンのページです。

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | 型              | 説明
|:---------------------|:------------------|:----------------------------------
| id                   | 文字列            | アイテムの一意識別子。読み取り専用です。
| name                 | string            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| eTag                 | string            | アイテムの ETag。読み取り専用です。
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
[サイト]: site.md
webpart

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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
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
