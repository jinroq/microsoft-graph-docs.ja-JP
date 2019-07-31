---
author: daspek
description: ItemActivityTimeSet リソースは、アイテムに対するアクティビティがいつ発生したかに関する情報を提供します。
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c81bf7885ee1466e293236a987e90e21323daefd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010092"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="12824-103">ItemActivityTimeSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12824-103">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12824-104">**ItemActivityTimeSet** リソースは、アイテムに対する[アクティビティ][activity]がいつ発生したかに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="12824-104">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="12824-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12824-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="12824-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12824-106">Properties</span></span>

| <span data-ttu-id="12824-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="12824-107">Property name</span></span>    | <span data-ttu-id="12824-108">種類</span><span class="sxs-lookup"><span data-stu-id="12824-108">Type</span></span>           | <span data-ttu-id="12824-109">説明</span><span class="sxs-lookup"><span data-stu-id="12824-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="12824-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="12824-110">observedDateTime</span></span> | <span data-ttu-id="12824-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12824-111">DateTimeOffset</span></span> | <span data-ttu-id="12824-112">アクティビティの発生が確認されたとき。</span><span class="sxs-lookup"><span data-stu-id="12824-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="12824-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="12824-113">recordedDateTime</span></span> | <span data-ttu-id="12824-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12824-114">DateTimeOffset</span></span> | <span data-ttu-id="12824-115">アクティビティの確認がサービスに記録されたとき。</span><span class="sxs-lookup"><span data-stu-id="12824-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="12824-116">**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。</span><span class="sxs-lookup"><span data-stu-id="12824-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="12824-117">ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="12824-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="12824-118">後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="12824-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="12824-119">備考</span><span class="sxs-lookup"><span data-stu-id="12824-119">Remarks</span></span>

<span data-ttu-id="12824-120">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="12824-120">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
