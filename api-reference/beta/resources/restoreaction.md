---
author: daspek
description: <decription>
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 88adfd244e2f8460d6749333cc64a80bf4d47361
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008692"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="0308c-102">RestoreAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0308c-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0308c-103">[**itemActivity**][activity] に **RestoreAction** リソースがある場合、アクティビティがアイテムを復元したことを示します。</span><span class="sxs-lookup"><span data-stu-id="0308c-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="0308c-104">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0308c-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0308c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0308c-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="0308c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0308c-106">Properties</span></span>

<span data-ttu-id="0308c-107">なし。</span><span class="sxs-lookup"><span data-stu-id="0308c-107">None.</span></span> <span data-ttu-id="0308c-108">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0308c-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0308c-109">備考</span><span class="sxs-lookup"><span data-stu-id="0308c-109">Remarks</span></span>

<span data-ttu-id="0308c-110">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="0308c-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": []
}
-->
