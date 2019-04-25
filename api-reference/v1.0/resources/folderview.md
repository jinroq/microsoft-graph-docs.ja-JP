---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 01b9860284f87ea31a969055fe2bfc7da624d3b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564114"
---
# <a name="folderview-resource-type"></a>FolderView リソースの種類

**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。

これは、[driveItem][item-resource] リソースの [folder][folder-facet] プロパティから使用できます。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名         | 種類   | 説明
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | string | フォルダーの並べ替え方法。
| **sortOrder**         | string | true の場合は、アイテムが降順で並べ替えられることを示します。 それ以外の場合は、アイテムが昇順で並べ替えられます。
| **viewType**          | string | フォルダーを表すために使用されるビューの種類。

_sortBy_ プロパティを使用すると、**viewType** ファセットを優先するアプリケーションで、アイテムの並べ替え順序を制御できます。

### <a name="sortby-options"></a>sortBy オプション

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


### <a name="sortorder-options"></a>ソート順序オプション

**sortOrder** プロパティに定義されている値は次のとおりです。

| 値        | 説明
| ------------ | --------------------------------------------------------------
| `ascending`  | アイテムは、昇順で整列されます。
| `descending` | アイテムは、降順で整列されます。


### <a name="viewtype-options"></a>viewType オプション

**viewType** プロパティに定義されている値は次のとおりです。

| 値        | 説明
| ------------ | --------------------------------------------------------------
| `default`    | アプリケーションの既定のビューの種類。
| `icons`      | driveItem を表すためにアイコンを使用するビュー。
| `details`    | 各アイテムに関する追加の詳細を提示する、複数の列を持つビュー。
| `thumbnails` | アイテムを表すために driveItem の大きなサムネイルを使用するビュー。


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->
