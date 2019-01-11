---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: a0c55967ed7f7a397e0c8c0a4ce607921dc8a9f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830549"
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

| プロパティ名        | Type     | 説明
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | 文字列   | サイト コレクションのホスト名です。読み取り専用です。
| **dataLocationCode** | 文字列   | このサイト コレクションが存在する地域コード。 読み取り専用です。
| **root**             | [root][] | 存在する場合は、SharePoint 内のルート サイト コレクションがあることを示します。 読み取り専用です。

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
