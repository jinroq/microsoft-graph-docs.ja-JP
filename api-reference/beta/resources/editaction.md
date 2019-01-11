---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 78e4d1aff2003cc6d23580f4e52b46667cf6a9e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841707"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="bd7c7-102">EditAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd7c7-102">EditAction resource type</span></span>

> <span data-ttu-id="bd7c7-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd7c7-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd7c7-105">[**itemActivity**][activity] に **EditAction** リソースがある場合、アクティビティがアイテムを編集したことを示します。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-105">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="bd7c7-106">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="bd7c7-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd7c7-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="bd7c7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd7c7-108">Properties</span></span>

<span data-ttu-id="bd7c7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-109">None.</span></span> <span data-ttu-id="bd7c7-110">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="bd7c7-111">備考</span><span class="sxs-lookup"><span data-stu-id="bd7c7-111">Remarks</span></span>

<span data-ttu-id="bd7c7-112">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="bd7c7-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction"
} -->
