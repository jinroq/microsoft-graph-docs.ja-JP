---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
ms.openlocfilehash: ce8f964b336f648cd1432532eb85a69629eb2207
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071869"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="55555-102">RestoreAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55555-102">RestoreAction resource type</span></span>

> <span data-ttu-id="55555-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55555-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55555-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55555-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55555-105">[**itemActivity**][activity] に **RestoreAction** リソースがある場合、アクティビティがアイテムを復元したことを示します。</span><span class="sxs-lookup"><span data-stu-id="55555-105">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="55555-106">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="55555-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="55555-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55555-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="55555-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55555-108">Properties</span></span>

<span data-ttu-id="55555-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55555-109">None.</span></span> <span data-ttu-id="55555-110">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="55555-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="55555-111">備考</span><span class="sxs-lookup"><span data-stu-id="55555-111">Remarks</span></span>

<span data-ttu-id="55555-112">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="55555-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction"
} -->
