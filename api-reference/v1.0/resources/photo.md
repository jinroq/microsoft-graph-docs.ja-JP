---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: a4284caa7c20e266d87e22e9b3d729e17bc88abf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="photo-resource-type"></a>Photo リソース型

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
| **fNumber**             | Double         | カメラの絞り値。読み取り専用です。
| **exposureDenominator** | Double         | カメラの露出時間の分数の分母。読み取り専用です。
| **exposureNumerator**   | Double         | カメラの露出時間の分数の分子。読み取り専用です。
| **focalLength**         | Double         | カメラの焦点距離。読み取り専用です。
| **iso**                 | Int64          | カメラの ISO 値。読み取り専用です。

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
