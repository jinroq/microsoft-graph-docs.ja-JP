---
title: Yammer アクティビティ レポート
description: 組織内での活動のレベル、および yammer でのメッセージの投稿、送受信を行う一意のユーザーの数によって、組織の契約レベルを知ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d5953d8bd53158b2ec0532deb47c48028ba1b8c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523804"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="eaedb-103">Yammer アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="eaedb-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaedb-104">組織内での活動のレベル、および yammer でのメッセージの投稿、送受信を行う一意のユーザーの数によって、組織の契約レベルを知ることができます。</span><span class="sxs-lookup"><span data-stu-id="eaedb-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="eaedb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaedb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="eaedb-106">レポート</span><span class="sxs-lookup"><span data-stu-id="eaedb-106">Reports</span></span>

| <span data-ttu-id="eaedb-107">関数</span><span class="sxs-lookup"><span data-stu-id="eaedb-107">Function</span></span>                                 | <span data-ttu-id="eaedb-108">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eaedb-108">CSV return type</span></span> | <span data-ttu-id="eaedb-109">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="eaedb-109">JSON return type</span></span>                         | <span data-ttu-id="eaedb-110">説明</span><span class="sxs-lookup"><span data-stu-id="eaedb-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="eaedb-111">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="eaedb-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="eaedb-112">Stream</span><span class="sxs-lookup"><span data-stu-id="eaedb-112">Stream</span></span>          | [<span data-ttu-id="eaedb-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="eaedb-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="eaedb-114">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="eaedb-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="eaedb-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="eaedb-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="eaedb-116">Stream</span><span class="sxs-lookup"><span data-stu-id="eaedb-116">Stream</span></span>          | [<span data-ttu-id="eaedb-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="eaedb-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="eaedb-118">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="eaedb-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="eaedb-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="eaedb-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="eaedb-120">Stream</span><span class="sxs-lookup"><span data-stu-id="eaedb-120">Stream</span></span>          | [<span data-ttu-id="eaedb-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="eaedb-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="eaedb-122">Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="eaedb-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
