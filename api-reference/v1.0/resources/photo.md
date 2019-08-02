---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 写真
localization_priority: Normal
description: 写真リソースは、EXIF メタデータなどの写真とカメラのプロパティを driveItem で提供します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c86190768c10b04bb55f59104368089cf7c77b18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035500"
---
# <a name="photo-resource-type"></a>写真リソースの種類

**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->

```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>プロパティ

| プロパティ                | 型           | 説明
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | 写真の撮影日時を表します。読み取り専用です。
| **cameraMake**          | String         | カメラの製造元。読み取り専用です。
| **cameraModel**         | String         | カメラのモデル。読み取り専用です。
| **fNumber**             | 2 行分         | カメラの絞り値。読み取り専用です。
| **exposureDenominator** | 2 行分         | カメラの露出時間の分数の分母。読み取り専用です。
| **exposureNumerator**   | Double         | カメラの露出時間の分数の分子。読み取り専用です。
| **focalLength**         | 倍精度浮動小数点数         | カメラの焦点距離。読み取り専用です。
| **iso**                 | Int32          | カメラの ISO 値。読み取り専用です。

## <a name="remarks"></a>注釈

OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
