---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 68e6419206d03ba44cb34919ae46b8f1688d49a0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334634"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="fcf52-102">EditAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fcf52-102">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf52-103">[**itemActivity**][activity] に **EditAction** リソースがある場合、アクティビティがアイテムを編集したことを示します。</span><span class="sxs-lookup"><span data-stu-id="fcf52-103">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="fcf52-104">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fcf52-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fcf52-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fcf52-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="fcf52-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fcf52-106">Properties</span></span>

<span data-ttu-id="fcf52-107">なし。</span><span class="sxs-lookup"><span data-stu-id="fcf52-107">None.</span></span> <span data-ttu-id="fcf52-108">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="fcf52-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="fcf52-109">備考</span><span class="sxs-lookup"><span data-stu-id="fcf52-109">Remarks</span></span>

<span data-ttu-id="fcf52-110">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="fcf52-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->
