---
author: JeremyKelley
description: FolderView リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5238c749d509339cd0e922e49b7e2d4d2da3b23f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973549"
---
# <a name="folderview-resource-type"></a>FolderView リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。

このプロパティは、 [Drive item][item-resource]リソースの[folder][folder-facet]プロパティから使用できます。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名         | 種類   | 説明
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | string | フォルダーの並べ替え方法。
| **sortOrder**         | string | true の場合は、アイテムが降順で並べ替えられることを示します。 それ以外の場合は、アイテムが昇順で並べ替えられます。
| **viewType**          | string | フォルダーを表すために使用されるビューの種類。

_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。

### <a name="sortby-values"></a>sortBy の値

**sortBy** プロパティに定義されている値は次のとおりです。

| 値                    | 説明
| ------------------------ | --------------------------------------------------
| `default`                | アプリケーションの既定の並べ替え順序。
| `name`                   | アイテムは、アイテムの **name** プロパティで整列されます。
| `type`                   | アイテムは、アイテムの種類で整列されます。
| `size`                   | アイテムは、アイテムの **size** プロパティで整列されます。
| `takenOrCreatedDateTime` | アイテムは、**photo** ファセットの **takenDateTime** プロパティで整列されます。 これが使用できない場合は、**createdDateTime** プロパティが使用されます。
| `lastModifiedDateTime`   | アイテムは、アイテムの **lastModifiedDateTime** プロパティで整列されます。
| `sequence`               | アイテムは、ユーザーによって指定されたカスタム順序で並びます。


### <a name="sortorder-values"></a>sortOrder の値

**sortOrder** プロパティに定義されている値は次のとおりです。

| 値        | 説明
| ------------ | --------------------------------------------------------------
| `ascending`  | アイテムは、昇順で整列されます。
| `descending` | アイテムは、降順で整列されます。


### <a name="viewtype-values"></a>viewType の値

**viewType** プロパティに定義されている値は次のとおりです。

| 値        | 説明
| ------------ | --------------------------------------------------------------
| `default`    | アプリケーションの既定のビューの種類。
| `icons`      | driveItem を表すためにアイコンを使用するビュー。
| `details`    | 各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。
| `thumbnails` | アイテムを表すために driveItem の大きなサムネイルを使用するビュー。


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
