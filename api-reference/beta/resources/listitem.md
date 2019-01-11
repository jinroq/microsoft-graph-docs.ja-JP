---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.openlocfilehash: b2e151937d5e8db633edeb5d521d6e0c875b6d78
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866088"
---
# <a name="listitem-resource"></a>ListItem リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
| [作成][]                     | POST /items
| [削除][]                     | DELETE /items/{item-id}
| [更新][]                     | PATCH /items/{item-id}
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

| プロパティ名 | Type                | 説明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | このリスト アイテムのコンテンツ タイプ

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | Type              | 説明
|:---------------------|:------------------|:----------------------------------
| ID                   | 文字列            | アイテムの一意識別子。読み取り専用です。
| name                 | 文字列            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| createdDateTime      | DateTimeOffset    | アイテムが作成された日時。読み取り専用です。
| description          | 文字列            | アイテムの説明テキストです。
| eTag                 | 文字列            | アイテムの ETag。読み取り専用です。                                                          |
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
