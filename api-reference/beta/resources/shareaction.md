---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 02098dd5bee739a078d8d9e3e744f7282ccb20bd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343197"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="17659-102">ShareAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17659-102">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17659-103">**ShareAction** リソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="17659-103">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="17659-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17659-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="17659-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17659-105">Properties</span></span>

| <span data-ttu-id="17659-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="17659-106">Property name</span></span> | <span data-ttu-id="17659-107">種類</span><span class="sxs-lookup"><span data-stu-id="17659-107">Type</span></span>                       | <span data-ttu-id="17659-108">説明</span><span class="sxs-lookup"><span data-stu-id="17659-108">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="17659-109">recipients</span><span class="sxs-lookup"><span data-stu-id="17659-109">recipients</span></span>    | <span data-ttu-id="17659-110">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="17659-110">[identitySet][] collection</span></span> | <span data-ttu-id="17659-111">このアクションでアイテムが共有された相手の ID。</span><span class="sxs-lookup"><span data-stu-id="17659-111">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="17659-113">備考</span><span class="sxs-lookup"><span data-stu-id="17659-113">Remarks</span></span>

<span data-ttu-id="17659-114">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="17659-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
