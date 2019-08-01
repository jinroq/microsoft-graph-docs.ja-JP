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
# <a name="shareaction-resource-type"></a><span data-ttu-id="b3b1e-103">/アクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3b1e-103">shareAction resource type</span></span>

<span data-ttu-id="b3b1e-104">" **Sharepoint**の共有" アクションリソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b3b1e-104">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="b3b1e-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b3b1e-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b3b1e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3b1e-106">Properties</span></span>

| <span data-ttu-id="b3b1e-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b3b1e-107">Property name</span></span> | <span data-ttu-id="b3b1e-108">種類</span><span class="sxs-lookup"><span data-stu-id="b3b1e-108">Type</span></span>                       | <span data-ttu-id="b3b1e-109">説明</span><span class="sxs-lookup"><span data-stu-id="b3b1e-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b3b1e-110">recipients</span><span class="sxs-lookup"><span data-stu-id="b3b1e-110">recipients</span></span>    | <span data-ttu-id="b3b1e-111">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b3b1e-111">[identitySet][] collection</span></span> | <span data-ttu-id="b3b1e-112">このアクションでアイテムが共有された相手の ID。</span><span class="sxs-lookup"><span data-stu-id="b3b1e-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="b3b1e-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3b1e-114">JSON representation</span></span>

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
