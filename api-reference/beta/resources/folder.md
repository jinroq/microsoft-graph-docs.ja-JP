---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: フォルダー
localization_priority: Normal
ms.openlocfilehash: b78e6038a8f8f9a91883dd29faeebe3d5db3ca04
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481217"
---
# <a name="folder-resource-type"></a>Folder リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の **[DriveItems](driveitem.md)** は、他の DriveItems のコンテナーです。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ       | 種類           | 説明
|:---------------|:---------------|:-------------------------------------------
| **childCount** | Int64          | このコンテナーの中に含まれる子の数。
| **view**       | [folderView][] | フォルダーに推奨されるビューを定義するプロパティのコレクション。


## <a name="remarks"></a>備考 

DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
