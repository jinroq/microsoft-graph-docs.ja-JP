---
title: Skype for Business アクティビティ レポート
description: 組織全体にわたってアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577383"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="55364-104">Skype for Business アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="55364-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55364-105">組織全体にわたってアクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="55364-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="55364-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="55364-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="55364-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55364-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="55364-108">レポート</span><span class="sxs-lookup"><span data-stu-id="55364-108">Reports</span></span>

| <span data-ttu-id="55364-109">関数</span><span class="sxs-lookup"><span data-stu-id="55364-109">Function</span></span>                                 | <span data-ttu-id="55364-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="55364-110">CSV return type</span></span> | <span data-ttu-id="55364-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="55364-111">JSON return type</span></span>                         | <span data-ttu-id="55364-112">説明</span><span class="sxs-lookup"><span data-stu-id="55364-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="55364-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="55364-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="55364-114">Stream</span><span class="sxs-lookup"><span data-stu-id="55364-114">Stream</span></span>          | [<span data-ttu-id="55364-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="55364-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="55364-116">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="55364-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="55364-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="55364-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="55364-118">Stream</span><span class="sxs-lookup"><span data-stu-id="55364-118">Stream</span></span>          | [<span data-ttu-id="55364-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="55364-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="55364-120">Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="55364-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="55364-121">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="55364-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="55364-122">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="55364-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="55364-123">Stream</span><span class="sxs-lookup"><span data-stu-id="55364-123">Stream</span></span>          | [<span data-ttu-id="55364-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="55364-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="55364-125">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="55364-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="55364-126">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="55364-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
