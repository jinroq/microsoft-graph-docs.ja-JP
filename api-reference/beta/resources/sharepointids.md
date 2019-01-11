---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.openlocfilehash: 6c67c45b333ead1d427c5b15ddd4ed5925b84eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807813"
---
# <a name="sharepointids-resource-type"></a>SharePointIds リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。

**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ         | 種類         | 説明
|:-----------------|:-------------|:-------------------------------------------
| listId           | 文字列       | SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。
| listItemId       | 文字列       | 含まれているリスト内にあるアイテムの整数の識別子。
| listItemUniqueId | 文字列       | OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。
| siteId           | 文字列       | アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。
| siteUrl          | string (URL) | アイテムが含まれるサイトの SharePoint URL です。
| tenantId         | 文字列       | 借用地の一意の識別子 (guid)。
| webId            | 文字列       | アイテムのサイト (SPWeb) の一意識別子 (guid)。

## <a name="remarks"></a>備考

**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
