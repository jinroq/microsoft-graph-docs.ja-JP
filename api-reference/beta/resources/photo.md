---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: 91b893fe3d6c78e3c3e16cbc41c7d7543b08f8d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527627"
---
# <a name="photo-resource-type"></a>写真リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/photo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
