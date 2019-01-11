---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 2ff3e1a2356c43457fe251928728632bd2228b10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809893"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="ee8ff-102">ItemActivityTimeSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee8ff-102">ItemActivityTimeSet resource type</span></span>

> <span data-ttu-id="ee8ff-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee8ff-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee8ff-105">**ItemActivityTimeSet** リソースは、アイテムに対する[アクティビティ][activity]がいつ発生したかに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="ee8ff-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee8ff-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ee8ff-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee8ff-107">Properties</span></span>

| <span data-ttu-id="ee8ff-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ee8ff-108">Property name</span></span>    | <span data-ttu-id="ee8ff-109">Type</span><span class="sxs-lookup"><span data-stu-id="ee8ff-109">Type</span></span>           | <span data-ttu-id="ee8ff-110">説明</span><span class="sxs-lookup"><span data-stu-id="ee8ff-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="ee8ff-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8ff-111">observedDateTime</span></span> | <span data-ttu-id="ee8ff-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8ff-112">DateTimeOffset</span></span> | <span data-ttu-id="ee8ff-113">アクティビティの発生が確認されたとき。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="ee8ff-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8ff-114">recordedDateTime</span></span> | <span data-ttu-id="ee8ff-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8ff-115">DateTimeOffset</span></span> | <span data-ttu-id="ee8ff-116">アクティビティの確認がサービスに記録されたとき。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="ee8ff-117">**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="ee8ff-118">ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="ee8ff-119">後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="ee8ff-120">備考</span><span class="sxs-lookup"><span data-stu-id="ee8ff-120">Remarks</span></span>

<span data-ttu-id="ee8ff-121">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ee8ff-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
