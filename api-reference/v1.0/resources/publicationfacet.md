---
title: PublicationFacet リソースの種類
description: '**publicationFacet **リソースは、driveItemVersion または driveItem リソースの公開ステータスの詳細情報を提供します。'
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020775"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet リソースの種類

**publicationFacet **リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a>プロパティ

|   プロパティ    |  型  | 説明 |
| :------------ | :----- | :---------- |
| **level**     | String | このドキュメントの公開状況。 `published` または `checkout` のどちらかです。 読み取り専用です。  |
| **versionId** | String | 現在の呼び出し元に表示されているバージョンの一意識別子です。 読み取り専用です。  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
