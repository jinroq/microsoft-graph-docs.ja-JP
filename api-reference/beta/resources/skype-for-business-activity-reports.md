---
title: Skype for Business アクティビティ レポート
description: 組織全体でのアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: fcd23201732f1e0988853ae33cf08a24295a2647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008244"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="fee2d-104">Skype for Business アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="fee2d-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee2d-105">組織全体でのアクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="fee2d-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="fee2d-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="fee2d-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="fee2d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fee2d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="fee2d-108">レポート</span><span class="sxs-lookup"><span data-stu-id="fee2d-108">Reports</span></span>

| <span data-ttu-id="fee2d-109">関数</span><span class="sxs-lookup"><span data-stu-id="fee2d-109">Function</span></span>                                 | <span data-ttu-id="fee2d-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fee2d-110">CSV return type</span></span> | <span data-ttu-id="fee2d-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="fee2d-111">JSON return type</span></span>                         | <span data-ttu-id="fee2d-112">説明</span><span class="sxs-lookup"><span data-stu-id="fee2d-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="fee2d-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="fee2d-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="fee2d-114">Stream</span><span class="sxs-lookup"><span data-stu-id="fee2d-114">Stream</span></span>          | [<span data-ttu-id="fee2d-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fee2d-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="fee2d-116">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="fee2d-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="fee2d-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fee2d-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="fee2d-118">Stream</span><span class="sxs-lookup"><span data-stu-id="fee2d-118">Stream</span></span>          | [<span data-ttu-id="fee2d-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="fee2d-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="fee2d-120">Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="fee2d-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="fee2d-121">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="fee2d-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="fee2d-122">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fee2d-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="fee2d-123">Stream</span><span class="sxs-lookup"><span data-stu-id="fee2d-123">Stream</span></span>          | [<span data-ttu-id="fee2d-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fee2d-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="fee2d-125">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="fee2d-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="fee2d-126">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="fee2d-126">The report also includes the number of peer-to-peer sessions.</span></span> |
