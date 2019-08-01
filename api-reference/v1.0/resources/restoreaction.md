---
author: daspek
ms.author: dspektor
title: restoreAction リソースの種類
description: RestoreAction オブジェクトは、アイテムを復元したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1395ee284fa2f3ca16371c8282124c07c9b4bd73
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034658"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="1aa7c-103">restoreAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1aa7c-103">restoreAction resource type</span></span>

<span data-ttu-id="1aa7c-104">[**Itemactivity**][activity]に**restoreaction**リソースが存在することは、アクティビティがアイテムを復元したことを示します。</span><span class="sxs-lookup"><span data-stu-id="1aa7c-104">The presence of the **restoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="1aa7c-105">**注**: このリソースは、現在空です。</span><span class="sxs-lookup"><span data-stu-id="1aa7c-105">**Note**: This resource is currently empty.</span></span> <span data-ttu-id="1aa7c-106">将来的には、追加のプロパティが設定される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1aa7c-106">In the future, it might be populated with additional properties.</span></span>

><span data-ttu-id="1aa7c-107">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1aa7c-107">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1aa7c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aa7c-108">Properties</span></span>

<span data-ttu-id="1aa7c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1aa7c-109">None.</span></span> <span data-ttu-id="1aa7c-110">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="1aa7c-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1aa7c-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1aa7c-111">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

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
