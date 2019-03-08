---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: イメージ
localization_priority: Normal
ms.openlocfilehash: 67d8a836ce89732ffd1fd6cb51fe5d8690e073e9
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480825"
---
# <a name="image-resource-type"></a>イメージ リソースの種類

**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。

**注:** サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a>プロパティ

| プロパティ   | 種類  | 説明                                |
|:-----------|:------|:-------------------------------------------|
| **height** | Int32 | 省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。 |
| **width**  | Int32 | 省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。  |

## <a name="remarks"></a>注釈

OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテムに対して返されます。

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
