---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: sitepage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583404"
---
# <a name="sitepage-resource"></a>sitepage リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このリソースは、sitepages[リスト][]のページを表します。
これには、タイトル、レイアウト、および[webPart][]のコレクションが含まれています。

## <a name="tasks-on-a-page"></a>ページ上のタスク

**sitepage**リソースでは、次のタスクを使用できます。
以下のすべての例は、[サイト][]に関連し`https://graph.microsoft.com/{api-version}/sites/{site-id}`ています。例:。

| 共通タスク                     | HTTP メソッド
|:--------------------------------|:------------------------------
| [List pages][]                  | ページを取得する
| [ページを取得する][]                    | ページを取得する/ページ/{pagefrom id}
| [作成][]                      | 投稿/ページ
| [削除][]                      | 削除/ページ/{page¥ id}
| [Publish][]                     | 投稿/ページ/_ page/発行

[List pages]: ../api/sitepage-list.md
[ページを取得する]: ../api/sitepage-get.md
[作成]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>JSON 表記

ここでは、 **sitepage**リソースの JSON 表記を示します。

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

**sitepage**リソースには、次のプロパティがあります。

| プロパティ名    | 種類                         | 説明
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | ページのコンテンツタイプ。

## <a name="page-content"></a>ページのコンテンツ

**sitepage**リソースには、次のコンテンツフィールドがあります。

| プロパティ名      | 種類                       | 説明
|:-------------------|:---------------------------|:---------------------------
| title              | string                     | ページのタイトル。
| pageLayout         | string                     | ページのページレイアウトの名前を指定します。
| パーツ           | [パーツ][]                | ページ上の web パーツ。

## <a name="authoring-metadata"></a>メタデータを作成する

**sitepage**リソースには、次の作成関連のメタデータがあります。 発行状態プロパティは、チェックアウトまたは発行されたページ作成状態を反映します。

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

**sitepage**リソースには、他のリソースとの関係がありません。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
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
