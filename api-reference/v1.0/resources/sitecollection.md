---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 98f7b9d930ccf7f1f0e1a6a0e1ad0353d49cf2bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022417"
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
| **root**             | [root][] | 存在する場合は、SharePoint 内のルート サイト コレクションがあることを示します。 読み取り専用。

[ルート]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
