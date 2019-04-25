---
title: Skype for Business アクティビティ レポート
description: 組織全体でのアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551905"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="e444b-104">Skype for Business アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="e444b-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e444b-105">組織全体でのアクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="e444b-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="e444b-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e444b-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="e444b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e444b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="e444b-108">レポート</span><span class="sxs-lookup"><span data-stu-id="e444b-108">Reports</span></span>

| <span data-ttu-id="e444b-109">関数</span><span class="sxs-lookup"><span data-stu-id="e444b-109">Function</span></span>                                 | <span data-ttu-id="e444b-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e444b-110">CSV return type</span></span> | <span data-ttu-id="e444b-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="e444b-111">JSON return type</span></span>                         | <span data-ttu-id="e444b-112">説明</span><span class="sxs-lookup"><span data-stu-id="e444b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e444b-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="e444b-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="e444b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="e444b-114">Stream</span></span>          | [<span data-ttu-id="e444b-115">skypeforbusinessactivityuserdetail</span><span class="sxs-lookup"><span data-stu-id="e444b-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="e444b-116">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e444b-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="e444b-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e444b-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="e444b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="e444b-118">Stream</span></span>          | [<span data-ttu-id="e444b-119">skypeforbusinessactivitycounts</span><span class="sxs-lookup"><span data-stu-id="e444b-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="e444b-120">Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="e444b-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="e444b-121">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="e444b-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="e444b-122">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e444b-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="e444b-123">Stream</span><span class="sxs-lookup"><span data-stu-id="e444b-123">Stream</span></span>          | [<span data-ttu-id="e444b-124">skypeforbusinessactivityusercounts</span><span class="sxs-lookup"><span data-stu-id="e444b-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="e444b-125">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="e444b-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="e444b-126">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="e444b-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
