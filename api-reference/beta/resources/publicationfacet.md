---
author: JeremyKelley
description: publicationFacet リソースは、driveItemVersion または driveItem リソースの公開ステータスの詳細情報を提供します。
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9c09f0863376e1569fb4af0acc0044fa1c7c8cfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008860"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| **versionId** | String | 現在の呼び出し元に表示されているバージョンの一意識別子です。 値の取得のみ可能です。  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
