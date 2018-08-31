---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 13ddb00d90880570361c7dcbe198c7c90e044957
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264400"
---
# <a name="listitem-resource"></a>ListItem リソース

このリソースは、SharePoint の **[list][]** 内のアイテムを表します。
リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。

## <a name="tasks-on-a-listitem"></a>listItem に関するタスク

**listItem** リソースで使用可能なタスクを次に示します。
以下のすべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。

| 共通タスク                    | HTTP メソッド
|:-------------------------------|:------------------------
| [取得][]                        | GET /items/{item-id}
| [列の値の取得][取得]       | GET /items/{item-id}?expand=fields
| [作成][]                     | POST /items
| [削除][]                     | DELETE /items/{item-id}
| [更新][]                     | PATCH /items/{item-id}
| [列の値の更新][更新] | PATCH /items/{item-id}/fields

[取得]: ../api/listItem_get.md
[作成]: ../api/listItem_create.md
[削除]: ../api/listItem_delete.md
[更新]: ../api/listItem_update.md

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
| ID                   | 文字列            | アイテムの一意識別子。読み取り専用です。
| 名前                 | 文字列            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| createdDateTime      | DateTimeOffset    | アイテムが作成された日時。読み取り専用です。
| 説明          | 文字列            | アイテムの説明テキストです。
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
| driveItem         | [driveItem][]                  | ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。
| フィールド            | [fieldValueSet][]              | このリスト アイテムの列セットの値です。
| バージョン          | [listItemVersion][] コレクション | リスト項目の以前のバージョンの一覧です。

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[リスト]: list.md
[listItemVersion]: listItemVersion.md
[sharepointIds]: sharepointIds.md

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
