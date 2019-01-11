---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 4cb3a56b5bdb4c3e7c9fc9fe69c0b34cae134a0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805608"
---
# <a name="publicationfacet-resource-type"></a>PublicationFacet リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

|   プロパティ    |  種類  | 説明 |
| :------------ | :----- | :---------- |
| **level**     | String | このドキュメントの公開状況。 `published` または `checkout` のどちらかです。 読み取り専用です。  |
| **versionId** | String | 現在の呼び出し元に表示されているバージョンの一意識別子です。 読み取り専用です。  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
