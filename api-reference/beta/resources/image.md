---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: c9e647ef630e8822d835aec1bd72b9f3c18f2e3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071531"
---
# <a name="image-resource-type"></a>イメージ リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ   | 型  | 説明                                |
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
