---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: プログラム
localization_priority: Normal
description: " または、個別のアイテムではなく、コレクションとして扱われるアイテムのコレクションです。"
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d8eff13e0cfdc6b355cc289833e7b3050ded2641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035666"
---
# <a name="package-resource-type"></a>Package リソースの種類

**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。

OneNote のノートブックはパッケージの一例です。ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。

**package** ファセットを持つ DriveItems は、**folder** や **file** ファセットを含みませんが、**folder** ファセットを持つ項目に概念的に類似しています。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 型   | 説明                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| type          | string | パッケージの種類を示す文字列。 が唯一の現在定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それぞれに応じた扱いをする必要があります。 |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
