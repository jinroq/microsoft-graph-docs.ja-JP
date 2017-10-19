---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 36636ead90d8b913de4328aea9b6252e82f30c26
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="sharepointids-resource-type"></a>SharePointIds リソース型

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
    "webId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ         | 型         | 説明
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。
| listItemId       | string       | 含まれているリスト内にあるアイテムの整数の識別子。
| listItemUniqueId | string       | OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。
| siteId           | string       | アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。
| siteUrl          | string (URL) | アイテムが含まれるサイトの SharePoint URL です。
| webId            | string       | アイテムのサイト (SPWeb) の一意識別子 (guid)。

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
