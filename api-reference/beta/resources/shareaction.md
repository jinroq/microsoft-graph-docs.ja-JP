---
author: daspek
description: ShareAction リソースは、アイテムを共有したアクティビティに関する情報を提供します。
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 10eb5b870a5ecd80f4a064d1dca496f216bf241d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965167"
---
# <a name="shareaction-resource-type"></a>ShareAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ShareAction** リソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類                       | 説明
|:--------------|:---------------------------|:-----------------------------
| recipients    | [identitySet][] コレクション | このアクションでアイテムが共有された相手の ID。

[identitySet]: identityset.md

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->
