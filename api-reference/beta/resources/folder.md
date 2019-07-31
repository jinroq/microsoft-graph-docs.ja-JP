---
author: JeremyKelley
description: 'Folder リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。 '
ms.date: 09/10/2017
title: フォルダー
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f9cbbba6ae20c56800a5f6f492319f47b7d8017c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971992"
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

| プロパティ       | 型           | 説明
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
  "suppressions": []
}
-->
