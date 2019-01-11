---
title: plannerFavoritePlanReference リソースの種類
description: '**PlannerFavoritePlanReference**リソースは、ユーザーがお気に入りとしてマークされている plannerPlan への参照の repesents を入力します。 '
localization_priority: Normal
ms.openlocfilehash: b17846eaa1b9a9859d23735d18a191cae4872542
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871324"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="e2af5-103">plannerFavoritePlanReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2af5-103">plannerFavoritePlanReference resource type</span></span>

> <span data-ttu-id="e2af5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2af5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2af5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2af5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2af5-106">**PlannerFavoritePlanReference**リソースは、ユーザーがお気に入りとしてマークされている[plannerPlan](plannerplan.md)への参照の repesents を入力します。</span><span class="sxs-lookup"><span data-stu-id="e2af5-106">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="e2af5-107">クライアントでは、 **plannerFavoritePlanReference**のエントリが削除する、ユーザーがアクセスできる不要になった、または別のタイトルで更新された**plannerPlans**を参照できるように注意してください。</span><span class="sxs-lookup"><span data-stu-id="e2af5-107">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="e2af5-108">クライアントは不一致がある場合にユーザーに通知し、エントリを常に最新の状態に保つことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e2af5-108">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="e2af5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2af5-109">Properties</span></span>
| <span data-ttu-id="e2af5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2af5-110">Property</span></span>     | <span data-ttu-id="e2af5-111">種類</span><span class="sxs-lookup"><span data-stu-id="e2af5-111">Type</span></span>   |<span data-ttu-id="e2af5-112">説明</span><span class="sxs-lookup"><span data-stu-id="e2af5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2af5-113">orderHint</span><span class="sxs-lookup"><span data-stu-id="e2af5-113">orderHint</span></span>|<span data-ttu-id="e2af5-114">String</span><span class="sxs-lookup"><span data-stu-id="e2af5-114">String</span></span>|<span data-ttu-id="e2af5-p103">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](planner-order-hint-format.md)」で定義されています。</span><span class="sxs-lookup"><span data-stu-id="e2af5-p103">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e2af5-117">planTitle</span><span class="sxs-lookup"><span data-stu-id="e2af5-117">planTitle</span></span>|<span data-ttu-id="e2af5-118">String</span><span class="sxs-lookup"><span data-stu-id="e2af5-118">String</span></span>|<span data-ttu-id="e2af5-119">ユーザーは、お気に入りとしてマークされている時にプランのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="e2af5-119">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e2af5-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2af5-120">JSON representation</span></span>

<span data-ttu-id="e2af5-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2af5-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
