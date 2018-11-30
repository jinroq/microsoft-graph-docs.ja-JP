---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: d54246002c158270ae23cf81cdc93673f40bd78c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070217"
---
# <a name="sitecollection-resource"></a>SiteCollection リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**siteCollection** リソースは、サイト コレクションの詳細を提供します。

[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ名        | 型     | 説明
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | 文字列   | サイト コレクションのホスト名です。読み取り専用です。
| **dataLocationCode** | 文字列   | このサイト コレクションが存在する地域コード。 読み取り専用。
| **root**             | [root][] | 存在する場合は、SharePoint 内のルート サイト コレクションがあることを示します。 読み取り専用。

[ルート]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
