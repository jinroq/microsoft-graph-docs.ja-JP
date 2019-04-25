---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 474d20e08d96294a30029e764d0b01f5b0c6bfcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581615"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="62975-102">ItemActivityTimeSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62975-102">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62975-103">**ItemActivityTimeSet** リソースは、アイテムに対する[アクティビティ][activity]がいつ発生したかに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="62975-103">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="62975-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62975-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="62975-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62975-105">Properties</span></span>

| <span data-ttu-id="62975-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="62975-106">Property name</span></span>    | <span data-ttu-id="62975-107">種類</span><span class="sxs-lookup"><span data-stu-id="62975-107">Type</span></span>           | <span data-ttu-id="62975-108">説明</span><span class="sxs-lookup"><span data-stu-id="62975-108">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="62975-109">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="62975-109">observedDateTime</span></span> | <span data-ttu-id="62975-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62975-110">DateTimeOffset</span></span> | <span data-ttu-id="62975-111">アクティビティの発生が確認されたとき。</span><span class="sxs-lookup"><span data-stu-id="62975-111">When the activity was observed to take place.</span></span>
| <span data-ttu-id="62975-112">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="62975-112">recordedDateTime</span></span> | <span data-ttu-id="62975-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62975-113">DateTimeOffset</span></span> | <span data-ttu-id="62975-114">アクティビティの確認がサービスに記録されたとき。</span><span class="sxs-lookup"><span data-stu-id="62975-114">When the observation was recorded on the service.</span></span>

<span data-ttu-id="62975-115">**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。</span><span class="sxs-lookup"><span data-stu-id="62975-115">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="62975-116">ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="62975-116">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="62975-117">後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="62975-117">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="62975-118">備考</span><span class="sxs-lookup"><span data-stu-id="62975-118">Remarks</span></span>

<span data-ttu-id="62975-119">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="62975-119">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitytimeset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
