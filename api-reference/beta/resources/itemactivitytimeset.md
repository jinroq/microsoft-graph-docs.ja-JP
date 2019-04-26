---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 999949f788c215a1e0645577a14b540586108926
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345417"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="4d651-102">ItemActivityTimeSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d651-102">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d651-103">**ItemActivityTimeSet** リソースは、アイテムに対する[アクティビティ][activity]がいつ発生したかに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4d651-103">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="4d651-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d651-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="4d651-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d651-105">Properties</span></span>

| <span data-ttu-id="4d651-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4d651-106">Property name</span></span>    | <span data-ttu-id="4d651-107">種類</span><span class="sxs-lookup"><span data-stu-id="4d651-107">Type</span></span>           | <span data-ttu-id="4d651-108">説明</span><span class="sxs-lookup"><span data-stu-id="4d651-108">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="4d651-109">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d651-109">observedDateTime</span></span> | <span data-ttu-id="4d651-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d651-110">DateTimeOffset</span></span> | <span data-ttu-id="4d651-111">アクティビティの発生が確認されたとき。</span><span class="sxs-lookup"><span data-stu-id="4d651-111">When the activity was observed to take place.</span></span>
| <span data-ttu-id="4d651-112">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d651-112">recordedDateTime</span></span> | <span data-ttu-id="4d651-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d651-113">DateTimeOffset</span></span> | <span data-ttu-id="4d651-114">アクティビティの確認がサービスに記録されたとき。</span><span class="sxs-lookup"><span data-stu-id="4d651-114">When the observation was recorded on the service.</span></span>

<span data-ttu-id="4d651-115">**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。</span><span class="sxs-lookup"><span data-stu-id="4d651-115">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="4d651-116">ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4d651-116">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="4d651-117">後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4d651-117">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="4d651-118">備考</span><span class="sxs-lookup"><span data-stu-id="4d651-118">Remarks</span></span>

<span data-ttu-id="4d651-119">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d651-119">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
