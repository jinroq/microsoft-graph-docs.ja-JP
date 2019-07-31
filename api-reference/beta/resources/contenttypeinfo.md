---
author: daspek
description: ContentTypeInfo リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 04316b01c905acb4fe38923f8d664ea892773e8e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012850"
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
