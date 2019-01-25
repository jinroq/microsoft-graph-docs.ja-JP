---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2a405ad8a71c766642bd23adbce64c2b57b72e23
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517443"
---
# <a name="listitem-resource"></a>ListItem リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このリソースは、SharePoint の **[list][]** 内のアイテムを表します。
リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。

## <a name="tasks-on-a-listitem"></a>listItem に関するタスク

**listItem** リソースで使用可能なタスクを次に示します。
以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。

| 共通タスク                    | HTTP メソッド
|:-------------------------------|:------------------------
| [取得][]                        | GET /items/{item-id}
| [列の値の取得][取得]       | GET /items/{item-id}?expand=fields
| [分析を取得します。][]              | GET/items/{アイテム id}/分析
| [間隔によってアクティビティを取得します。][] | GET/items/{アイテム id}/getActivitiesByInterval
| [Create][]                     | POST /items
| [Delete][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [列の値の更新][更新] | PATCH /items/{item-id}/fields

[取得]: ../api/listitem-get.md
[分析を取得します。]: ../api/itemanalytics-get.md
[間隔によってアクティビティを取得します。]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md

## <a name="json-representation"></a>JSON 表記

以下は、**listItem** リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

**listItem** リソースには以下のプロパティがあります。

| プロパティ名 | 型                | 説明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | このリスト アイテムのコンテンツ タイプ

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | 型              | 説明
|:---------------------|:------------------|:----------------------------------
| id                   | 文字列            | アイテムの一意識別子。読み取り専用です。
| name                 | string            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| createdDateTime      | DateTimeOffset    | アイテムが作成された日時。読み取り専用です。
| 説明          | string            | アイテムの説明テキストです。
| eTag                 | string            | アイテムの ETag。読み取り専用です。                                                          |
| lastModifiedBy       | [identitySet][]   | このアイテムの最終変更者の ID です。 読み取り専用です。
| lastModifiedDateTime | DateTimeOffset    | アイテムが最後に変更された日時。読み取り専用です。
| parentReference      | [itemReference][] | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。
| sharepointIds        | [sharepointIds][] | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。
| webUrl               | string (URL)      | ブラウザーでアイテムを表示する URL。読み取り専用です。

## <a name="relationships"></a>リレーションシップ

 **listItem** リソースには、他のリソースと次のような関係があります。

| リレーションシップ名 | 種類                           | 説明
|:------------------|:-------------------------------|:-------------------------------
| アクティビティ        | [itemActivity][] コレクション    | このアイテムに対して行われた最近のアクティビティのリストです。
| 分析         | [itemAnalytics][]リソース     | この項目に対して行われた活動の表示について分析します。
| driveItem         | [driveItem][]                  | ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。
| fields            | [fieldValueSet][]              | このリスト アイテムの列セットの値です。
| versions          | [listItemVersion][]コレクション | リスト項目の以前のバージョンの一覧です。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[リスト]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
