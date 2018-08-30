---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: パッケージ
ms.openlocfilehash: 12ae750a0f4fbe0e951554308d4041928c31a16d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267543"
---
# <a name="package-resource-type"></a>Package リソースの種類

**Package** リソースは、DriveItem が「パッケージ」内で最上位項目であること、または個別の項目ではなくコレクションとして扱うべき項目のコレクションであることを示します。

OneNote のノートブックはパッケージの一例です。 ノートブックがその内容を表すファイルとフォルダーで構成されているのに対し、ノートブックを表す最上位項目は、これが特別な扱いを必要とするデータのコレクションであることをクライアントに示す **package** ファセットを持ちます。

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
| 型          | 文字列 | パッケージのタイプを示す文字列です。 `oneNote` が現在唯一定義されている値であるとしても、他のパッケージ タイプが返されるものと考え、それに応じて対応する必要があります。 |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
