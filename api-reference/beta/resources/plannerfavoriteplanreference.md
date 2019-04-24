---
title: プラン "お気に入り" プラン参照リソースの種類
description: 'プラン [**参照**リソースの種類表す workbookconnection は、ユーザーによってお気に入りとしてマークされているプランへの参照を示します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77a931a882cc4b01725bd8ceb0ae6bcc721a9013
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457103"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="704fd-103">プラン "お気に入り" プラン参照リソースの種類</span><span class="sxs-lookup"><span data-stu-id="704fd-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="704fd-104">プラン [**参照**リソースの種類表す workbookconnection は、ユーザーによってお気に入りとしてマークされている[プラン](plannerplan.md)への参照を示します。</span><span class="sxs-lookup"><span data-stu-id="704fd-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="704fd-105">クライアントは、「 \*\*\*\* プラン」では、削除されたプラン、ユーザーがアクセスできなくなったプラン、または別のタイトルで更新された**プラン**を参照することができることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="704fd-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="704fd-106">クライアントは、相違点がある場合にユーザーに通知し、エントリを最新の状態に維持することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="704fd-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="704fd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="704fd-107">Properties</span></span>
| <span data-ttu-id="704fd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="704fd-108">Property</span></span>     | <span data-ttu-id="704fd-109">型</span><span class="sxs-lookup"><span data-stu-id="704fd-109">Type</span></span>   |<span data-ttu-id="704fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="704fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="704fd-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="704fd-111">orderHint</span></span>|<span data-ttu-id="704fd-112">String</span><span class="sxs-lookup"><span data-stu-id="704fd-112">String</span></span>|<span data-ttu-id="704fd-p102">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](planner-order-hint-format.md)」で定義されています。</span><span class="sxs-lookup"><span data-stu-id="704fd-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="704fd-115">プランのタイトル</span><span class="sxs-lookup"><span data-stu-id="704fd-115">planTitle</span></span>|<span data-ttu-id="704fd-116">String</span><span class="sxs-lookup"><span data-stu-id="704fd-116">String</span></span>|<span data-ttu-id="704fd-117">ユーザーがお気に入りとしてマークした時点でのプランのタイトル。</span><span class="sxs-lookup"><span data-stu-id="704fd-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="704fd-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="704fd-118">JSON representation</span></span>

<span data-ttu-id="704fd-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="704fd-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
