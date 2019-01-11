---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: 98c477ebeda436c57db3eaac5cb062639a2447d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856498"
---
# <a name="folder-resource-type"></a>Folder リソース型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の [**DriveItems**](driveitem.md) は、他の DriveItems のコンテナーです。

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

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
