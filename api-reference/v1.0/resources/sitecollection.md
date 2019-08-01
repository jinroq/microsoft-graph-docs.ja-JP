---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: siteCollection リソースは、サイト コレクションの詳細を提供します。
doc_type: resourcePageType
ms.openlocfilehash: 27a534f2f9afe99a1a5abb1aee91b1b53b29566d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034161"
---
# <a name="sitecollection-resource"></a>SiteCollection リソース

**siteCollection** リソースは、サイト コレクションの詳細を提供します。

[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ名        | 種類     | 説明
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | string   | サイト コレクションのホスト名です。読み取り専用です。
| **root**             | [root][] | 存在する場合は、これが SharePoint のルートサイトコレクションであることを示します。 読み取り専用です。

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
