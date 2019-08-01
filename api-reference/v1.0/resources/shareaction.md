---
author: daspek
ms.author: dspektor
title: /アクションリソースの種類
description: Share Action オブジェクトは、共有アクションでアイテムが共有されたユーザーに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 73b847bbd9608a7647f3895e8d67fff9dbdc9a68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034350"
---
# <a name="shareaction-resource-type"></a>/アクションリソースの種類

" **Sharepoint**の共有" アクションリソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[activity]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類                       | 説明
|:--------------|:---------------------------|:-----------------------------
| recipients    | [identitySet][] コレクション | このアクションでアイテムが共有された相手の ID。

[identitySet]: identityset.md

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

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->
