---
title: Yammer アクティビティ レポート
description: Yammer に組織の活動のレベルを理解するには、組織、Yammer にメッセージを読むの投稿などのおよび一意のユーザー数の間でどの程度の活動が生成されます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509939"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="4bd91-103">Yammer アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="4bd91-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bd91-104">Yammer に組織の活動のレベルを理解するには、組織、Yammer にメッセージを読むの投稿などのおよび一意のユーザー数の間でどの程度の活動が生成されます。</span><span class="sxs-lookup"><span data-stu-id="4bd91-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="4bd91-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bd91-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="4bd91-106">レポート</span><span class="sxs-lookup"><span data-stu-id="4bd91-106">Reports</span></span>

| <span data-ttu-id="4bd91-107">関数</span><span class="sxs-lookup"><span data-stu-id="4bd91-107">Function</span></span>                                 | <span data-ttu-id="4bd91-108">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4bd91-108">CSV return type</span></span> | <span data-ttu-id="4bd91-109">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4bd91-109">JSON return type</span></span>                         | <span data-ttu-id="4bd91-110">説明</span><span class="sxs-lookup"><span data-stu-id="4bd91-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4bd91-111">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="4bd91-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="4bd91-112">Stream</span><span class="sxs-lookup"><span data-stu-id="4bd91-112">Stream</span></span>          | [<span data-ttu-id="4bd91-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4bd91-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="4bd91-114">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bd91-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="4bd91-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="4bd91-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="4bd91-116">Stream</span><span class="sxs-lookup"><span data-stu-id="4bd91-116">Stream</span></span>          | [<span data-ttu-id="4bd91-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="4bd91-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="4bd91-118">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bd91-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="4bd91-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="4bd91-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="4bd91-120">ストリーム</span><span class="sxs-lookup"><span data-stu-id="4bd91-120">Stream</span></span>          | [<span data-ttu-id="4bd91-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="4bd91-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="4bd91-122">Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bd91-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
