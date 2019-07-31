---
author: JeremyKelley
ms.author: jeremyke
title: バンドルリソースの種類
description: 他のドライブ項目の論理グループであるドライブ項目を記述するファセット
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f843afa112f95e391761d0c8804600018a67534c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974096"
---
# <a name="bundle-resource-type"></a>バンドルリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

バンドルとは、一度に複数のファイルを共有するために使用されるファイルの論理的なグループです。 ファセットが含まれている[ハードドライブ][]エンティティで表され、他のすべての drive アイテムと同じ方法で共有できます。 `bundle`

`bundle` [ドライブアイテム][]のファセットは、アイテムをバンドルとして識別し、バンドル固有の情報を1つの構造にグループ化します。 このファイルは、**バンドル**エンドポイントから返される[ドライブ項目][]リソースにのみ含まれます。

`bundle`リソースの種類自体は自身のエンティティではないことに注意してください。また、[ドライブアイテム][]のファセットでしかありません。 ドライブ`bundles`上のコレクション[][]の種類は、drive [item][]では`bundle`ありません。

## <a name="methods"></a>メソッド

|                        メソッド             |         戻り値の型      | 説明        |
| :---------------------------------------- | :----------------------- | :------------------|
| [リストバンドル][bundle-list]               | [driveItem][] コレクション | ドライブ内のすべてのバンドルを一覧表示する |
| [バンドルを取得する][bundle-get]                  | [driveItem][]            | バンドルメタデータを取得する |
| [バンドルを作成する][bundle-create]            | [driveItem][]            | 新しいバンドルを作成する |
| [アイテムを追加する][bundle-add-item]               | None                     | 既存のバンドルに[ドライブ項目][]を追加する |
| [アイテムの削除][bundle-remove-item]         | None                     | 既存のバンドルからの[ドライブ項目][]の削除 |
| [バンドルの更新][bundle-update]            | [driveItem][]            | バンドルメタデータの更新 |
| [バンドルの削除][bundle-delete]            | None                     | バンドルの削除 |


## <a name="properties"></a>プロパティ

| プロパティ名 | 種類      | 説明
|:--------------|:----------|:------------------------------------------------
| childCount    | Int32     | このコンテナーの中に含まれる子の数。
| album         | [album][] | バンドルが[アルバム][]の場合は、プロパティが`album`含まれます。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.bundle" } -->
```json
{
  "childCount": 3,
  "album": { "@odata.type": "microsoft.graph.album" },
}
```

[album]: album.md
[drive]: drive.md
[driveItem]: driveItem.md

[bundle-list]: ../api/bundle-list.md
[bundle-get]: ../api/bundle-get.md
[bundle-create]: ../api/drive-post-bundles.md
[bundle-add-item]: ../api/bundle-addItem.md
[bundle-remove-item]: ../api/bundle-removeItem.md
[bundle-update]: ../api/bundle-update.md
[bundle-delete]: ../api/bundle-delete.md
