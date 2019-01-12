---
title: Yammer アクティビティ レポート
description: Yammer に組織の活動のレベルを理解するには、組織、Yammer にメッセージを読むの投稿などのおよび一意のユーザー数の間でどの程度の活動が生成されます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 69c155df86cfe772e0c065bec0297a83fb7f3a8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912037"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="3ceb6-103">Yammer アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="3ceb6-103">Yammer activity reports</span></span>

> <span data-ttu-id="3ceb6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ceb6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="3ceb6-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="3ceb6-107">Yammer に組織の活動のレベルを理解するには、組織、Yammer にメッセージを読むの投稿などのおよび一意のユーザー数の間でどの程度の活動が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-107">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="3ceb6-108">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="3ceb6-109">レポート</span><span class="sxs-lookup"><span data-stu-id="3ceb6-109">Reports</span></span>

| <span data-ttu-id="3ceb6-110">関数</span><span class="sxs-lookup"><span data-stu-id="3ceb6-110">Function</span></span>                                 | <span data-ttu-id="3ceb6-111">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3ceb6-111">CSV return type</span></span> | <span data-ttu-id="3ceb6-112">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3ceb6-112">JSON return type</span></span>                         | <span data-ttu-id="3ceb6-113">説明</span><span class="sxs-lookup"><span data-stu-id="3ceb6-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="3ceb6-114">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="3ceb6-114">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="3ceb6-115">Stream</span><span class="sxs-lookup"><span data-stu-id="3ceb6-115">Stream</span></span>          | [<span data-ttu-id="3ceb6-116">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="3ceb6-116">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="3ceb6-117">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-117">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="3ceb6-118">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="3ceb6-118">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="3ceb6-119">Stream</span><span class="sxs-lookup"><span data-stu-id="3ceb6-119">Stream</span></span>          | [<span data-ttu-id="3ceb6-120">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="3ceb6-120">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="3ceb6-121">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-121">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="3ceb6-122">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="3ceb6-122">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="3ceb6-123">Stream</span><span class="sxs-lookup"><span data-stu-id="3ceb6-123">Stream</span></span>          | [<span data-ttu-id="3ceb6-124">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="3ceb6-124">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="3ceb6-125">Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="3ceb6-125">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
