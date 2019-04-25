---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: f82242da39ebc13d769a0a3471b60dd4ac9df8dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542320"
---
# <a name="folderview-resource-type"></a>FolderView リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**FolderView** リソースは、フォルダーのユーザー エクスペリエンスに関する推奨事項を提供または設定します。

これは、[driveItem][item-resource] リソースの [folder][folder-facet] プロパティから使用できます。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
