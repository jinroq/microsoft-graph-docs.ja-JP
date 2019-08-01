---
author: daspek
ms.author: dspektor
title: itemActivityTimeSet リソースの種類
description: ItemActionSet オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9dce21afc1acc8e93181204e026f74a597c9120f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036590"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="15189-103">itemActivityTimeSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15189-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="15189-104">**Itemactivitytimeset**リソースは、アイテムの[アクティビティ][activity]が実行された日時に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="15189-104">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="15189-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="15189-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="15189-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15189-106">Properties</span></span>

| <span data-ttu-id="15189-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="15189-107">Property name</span></span>    | <span data-ttu-id="15189-108">種類</span><span class="sxs-lookup"><span data-stu-id="15189-108">Type</span></span>           | <span data-ttu-id="15189-109">説明</span><span class="sxs-lookup"><span data-stu-id="15189-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="15189-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="15189-110">observedDateTime</span></span> | <span data-ttu-id="15189-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15189-111">DateTimeOffset</span></span> | <span data-ttu-id="15189-112">アクティビティの発生が確認されたとき。</span><span class="sxs-lookup"><span data-stu-id="15189-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="15189-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="15189-113">recordedDateTime</span></span> | <span data-ttu-id="15189-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15189-114">DateTimeOffset</span></span> | <span data-ttu-id="15189-115">アクティビティの確認がサービスに記録されたとき。</span><span class="sxs-lookup"><span data-stu-id="15189-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="15189-116">**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。</span><span class="sxs-lookup"><span data-stu-id="15189-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="15189-117">ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="15189-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="15189-118">後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="15189-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15189-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15189-119">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
