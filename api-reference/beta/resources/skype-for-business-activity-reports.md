---
title: Skype for Business アクティビティ レポート
description: 組織全体にわたってアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a81e27d58316cb415d6296b4f77519a3f2125643
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512396"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="557d9-104">Skype for Business アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="557d9-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="557d9-105">組織全体にわたってアクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="557d9-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="557d9-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="557d9-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="557d9-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="557d9-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="557d9-108">レポート</span><span class="sxs-lookup"><span data-stu-id="557d9-108">Reports</span></span>

| <span data-ttu-id="557d9-109">関数</span><span class="sxs-lookup"><span data-stu-id="557d9-109">Function</span></span>                                 | <span data-ttu-id="557d9-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="557d9-110">CSV return type</span></span> | <span data-ttu-id="557d9-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="557d9-111">JSON return type</span></span>                         | <span data-ttu-id="557d9-112">説明</span><span class="sxs-lookup"><span data-stu-id="557d9-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="557d9-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="557d9-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="557d9-114">Stream</span><span class="sxs-lookup"><span data-stu-id="557d9-114">Stream</span></span>          | [<span data-ttu-id="557d9-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="557d9-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="557d9-116">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="557d9-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="557d9-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="557d9-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="557d9-118">Stream</span><span class="sxs-lookup"><span data-stu-id="557d9-118">Stream</span></span>          | [<span data-ttu-id="557d9-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="557d9-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="557d9-120">Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="557d9-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="557d9-121">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="557d9-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="557d9-122">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="557d9-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="557d9-123">ストリーム</span><span class="sxs-lookup"><span data-stu-id="557d9-123">Stream</span></span>          | [<span data-ttu-id="557d9-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="557d9-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="557d9-125">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="557d9-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="557d9-126">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="557d9-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
