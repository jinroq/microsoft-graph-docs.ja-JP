---
author: daspek
description: itemActivity に EditAction リソースがある場合、アクティビティがアイテムを編集したことを示します。
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 374b4f7374ba91360bdaa97e5bc36fb0f5aabbae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006508"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="b200a-103">EditAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b200a-103">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b200a-104">[**itemActivity**][activity] に **EditAction** リソースがある場合、アクティビティがアイテムを編集したことを示します。</span><span class="sxs-lookup"><span data-stu-id="b200a-104">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="b200a-105">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b200a-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b200a-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b200a-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="b200a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b200a-107">Properties</span></span>

<span data-ttu-id="b200a-108">なし。</span><span class="sxs-lookup"><span data-stu-id="b200a-108">None.</span></span> <span data-ttu-id="b200a-109">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="b200a-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="b200a-110">備考</span><span class="sxs-lookup"><span data-stu-id="b200a-110">Remarks</span></span>

<span data-ttu-id="b200a-111">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b200a-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
