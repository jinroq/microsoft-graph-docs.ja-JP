---
author: JeremyKelley
ms.author: JeremyKelley
title: ListItem リソース
description: このリソースは、SharePoint のリスト内のアイテムを表します。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 873ad5961c9cadb444c6fe9f2afec69853cc5d85
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968801"
---
# <a name="listitem-resource"></a>ListItem リソース

このリソースは、SharePoint の **[list][]** 内のアイテムを表します。
リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。

## <a name="methods"></a>メソッド

**listItem** リソースで使用可能なメソッドを次に示します。
すべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}` の**[リスト][]** からの相対指定です。

| メソッド                    | 戻り値の型 | 説明
|:-------------------------------|:-------------------|:------
| [Get][]                   | lisItem| リスト内のアイテムを取得する。
| [列の値 ][Get] を取得       | listItem | リスト アイテムから列の値を取得します。
| [分析を取得する][]              | [itemAnalytics][]| このリソースの分析を取得します。 
| [間隔ごとにアクティビティを取得する][] | [itemActivityStat][]| 指定した時間間隔内に itemActivityStats のコレクションを取得します。
| [作成する][]                     | listItem | リストに新しい listItem を作成します。
| [削除][]                     | コンテンツはありません | リストからアイテムを削除します。
| [更新][]                     | [fieldValueSet][]| リストアイテム のプロパティを更新します。
| [列の値 ][更新]を更新する | [fieldValueSet][]| リスト アイテムの列の値を更新します。

[取得]: ../api/listitem-get.md
[分析を取得する]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[削除]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a>プロパティ

**listItem** リソースには以下のプロパティがあります。

| プロパティ名 | 種類                | 説明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | このリスト アイテムのコンテンツ タイプ

次のプロパティは、**[baseItem][]** から継承しています。

| プロパティ名        | 種類              | 説明
|:---------------------|:------------------|:----------------------------------
| id                   | string            | アイテムの一意識別子。読み取り専用です。
| name                 | string            | アイテムの名前/タイトル。
| createdBy            | [identitySet][]   | このアイテムの作成者の ID です。 読み取り専用です。
| createdDateTime      | DateTimeOffset    | アイテムが作成された日時。読み取り専用です。
| description          | string            | アイテムの説明テキストです。
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
| 分析         | [itemAnalytics][] リソース     | このアイテムについて行われたビュー アクティビティに関する分析。
| driveItem         | [driveItem][]                  | ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。
| フィールド            | [fieldValueSet][]              | このリスト アイテムの列セットの値です。
| versions          | [listItemVersion][] コレクション | リスト アイテムの以前のバージョンのリスト。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
