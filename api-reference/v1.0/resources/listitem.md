---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2018
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

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

**listItem** リソースには以下のプロパティがあります。

| プロパティ名 | 種類                | 説明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | このリスト アイテムのコンテンツ タイプ
| fields        | [fieldValueSet][]   | このリスト アイテムの列セットの値です。

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | 種類             | 説明
|:---------------------|:-----------------|:-----------------------------------
| id                   | string           | アイテムの一意識別子。読み取り専用です。
| name                 | string           | アイテムの名前/タイトル。
| createdBy            | [identitySet][]  | このアイテムの作成者の ID です。 読み取り専用です。
| createdDateTime      | DateTimeOffset   | アイテムが作成された日時。読み取り専用です。
| description          | string           | アイテムの説明テキストです。
| lastModifiedBy       | [identitySet][]  | このアイテムの最終変更者の ID です。 読み取り専用です。
| lastModifiedDateTime | DateTimeOffset   | アイテムが最後に変更された日時。読み取り専用です。
| webUrl               | string (URL)     | ブラウザーでアイテムを表示する URL。読み取り専用です。

## <a name="relationships"></a>リレーションシップ

 **listItem** リソースには、他のリソースと次のような関係があります。

| リレーションシップ名 | 種類                        | 説明
|:------------------|:----------------------------|:-------------------------------
| driveItem         | [driveItem][]               | ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
