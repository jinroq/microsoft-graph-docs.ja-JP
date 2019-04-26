---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341229"
---
# <a name="contenttypeinfo-resource-type"></a>ContentTypeInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ContentTypeInfo** リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**contentTypeInfo** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名  | 種類    | 説明
|:---------------|:--------|:--------------------------------------------------
| **id**         | string  | コンテンツ タイプの ID。
| **name**       | string  | コンテンツ タイプの名前。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
