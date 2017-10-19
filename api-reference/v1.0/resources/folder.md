---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: 664597297700f7af096ef30cfbd5342a45a6c157
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="folder-resource-type"></a>Folder リソース型

**Folder** リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。 
null でない **folder** ファセットを持つ [**DriveItem**](driveitem.md) は、他の DriveItem のコンテナーです。

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

| プロパティ       | 型           | 説明
|:---------------|:---------------|:-------------------------------------------
| **childCount** | Int64          | このコンテナーの中に含まれる子の数。
| **view**       | [folderView][] | フォルダーに推奨されるビューを定義するプロパティのコレクション。

## <a name="remarks"></a>備考 

DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
