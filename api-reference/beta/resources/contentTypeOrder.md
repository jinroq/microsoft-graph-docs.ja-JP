---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 32cca632933cf2b0fad1f8e9149973d95b4322d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341233"
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。

## <a name="json-representation"></a>JSON 表記

以下は、**contentTypeOrder** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類    | 説明
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | 既定のコンテンツ タイプかどうか。
| **position**  | Int32   | コンテンツ タイプが選択 UI で表示される位置を指定します。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
