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
# <a name="shareaction-resource-type"></a><span data-ttu-id="921f3-103">ShareAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="921f3-103">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="921f3-104">**ShareAction** リソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="921f3-104">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="921f3-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="921f3-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="921f3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="921f3-106">Properties</span></span>

| <span data-ttu-id="921f3-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="921f3-107">Property name</span></span> | <span data-ttu-id="921f3-108">種類</span><span class="sxs-lookup"><span data-stu-id="921f3-108">Type</span></span>                       | <span data-ttu-id="921f3-109">説明</span><span class="sxs-lookup"><span data-stu-id="921f3-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="921f3-110">recipients</span><span class="sxs-lookup"><span data-stu-id="921f3-110">recipients</span></span>    | <span data-ttu-id="921f3-111">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="921f3-111">[identitySet][] collection</span></span> | <span data-ttu-id="921f3-112">このアクションでアイテムが共有された相手の ID。</span><span class="sxs-lookup"><span data-stu-id="921f3-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="921f3-114">備考</span><span class="sxs-lookup"><span data-stu-id="921f3-114">Remarks</span></span>

<span data-ttu-id="921f3-115">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="921f3-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
