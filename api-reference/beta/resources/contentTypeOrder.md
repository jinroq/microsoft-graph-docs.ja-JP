---
author: daspek
description: contentTypeOrder リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 464ac5978f505e74ca99226080c35574917fd550
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973206"
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
