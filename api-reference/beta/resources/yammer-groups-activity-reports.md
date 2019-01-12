---
title: Yammer グループ アクティビティ レポート
description: 組織で Yammer グループの活動の洞察を獲得でき、Yammer グループの数が表示されるを参照してください作成され、使用されます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e2726e55e089aa494eaf35d0948f0fa3948be781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950817"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="255b6-103">Yammer グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="255b6-103">Yammer groups activity reports</span></span>

> <span data-ttu-id="255b6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="255b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="255b6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="255b6-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="255b6-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="255b6-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="255b6-107">組織で Yammer グループの活動の洞察を獲得でき、Yammer グループの数が表示されるを参照してください作成され、使用されます。</span><span class="sxs-lookup"><span data-stu-id="255b6-107">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="255b6-108">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="255b6-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="255b6-109">レポート</span><span class="sxs-lookup"><span data-stu-id="255b6-109">Reports</span></span>

| <span data-ttu-id="255b6-110">関数</span><span class="sxs-lookup"><span data-stu-id="255b6-110">Function</span></span>                                 | <span data-ttu-id="255b6-111">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="255b6-111">CSV return type</span></span> | <span data-ttu-id="255b6-112">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="255b6-112">JSON return type</span></span>                         | <span data-ttu-id="255b6-113">説明</span><span class="sxs-lookup"><span data-stu-id="255b6-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="255b6-114">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="255b6-114">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="255b6-115">Stream</span><span class="sxs-lookup"><span data-stu-id="255b6-115">Stream</span></span>          | [<span data-ttu-id="255b6-116">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="255b6-116">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="255b6-117">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="255b6-117">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="255b6-118">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="255b6-118">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="255b6-119">Stream</span><span class="sxs-lookup"><span data-stu-id="255b6-119">Stream</span></span>          | [<span data-ttu-id="255b6-120">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="255b6-120">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="255b6-121">存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。</span><span class="sxs-lookup"><span data-stu-id="255b6-121">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="255b6-122">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="255b6-122">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="255b6-123">Stream</span><span class="sxs-lookup"><span data-stu-id="255b6-123">Stream</span></span>          | [<span data-ttu-id="255b6-124">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="255b6-124">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="255b6-125">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="255b6-125">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
