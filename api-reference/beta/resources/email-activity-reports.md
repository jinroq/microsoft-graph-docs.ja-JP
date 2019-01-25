---
title: 電子メール アクティビティ レポート
description: '[レポート] ページから、組織内で電子メール トラフィックの高レベルのビューを取得できます。 傾向と、組織内の電子メール活動のユーザーごとの詳細を理解する電子メール活動のウィジェットにドリルダウンすることもできます。'
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: e11de43f197e520d653961af9b9090d06b085369
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528306"
---
# <a name="email-activity-reports"></a><span data-ttu-id="0c008-104">電子メール アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="0c008-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c008-105">[レポート] ページから、組織内で電子メール トラフィックの高レベルのビューを取得できます。</span><span class="sxs-lookup"><span data-stu-id="0c008-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="0c008-106">傾向と、組織内の電子メール活動のユーザーごとの詳細を理解する電子メール活動のウィジェットにドリルダウンすることもできます。</span><span class="sxs-lookup"><span data-stu-id="0c008-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="0c008-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c008-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="0c008-108">レポート</span><span class="sxs-lookup"><span data-stu-id="0c008-108">Reports</span></span>

| <span data-ttu-id="0c008-109">関数</span><span class="sxs-lookup"><span data-stu-id="0c008-109">Function</span></span>                                 | <span data-ttu-id="0c008-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c008-110">CSV return type</span></span> | <span data-ttu-id="0c008-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c008-111">JSON return type</span></span>                         | <span data-ttu-id="0c008-112">説明</span><span class="sxs-lookup"><span data-stu-id="0c008-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0c008-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="0c008-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="0c008-114">Stream</span><span class="sxs-lookup"><span data-stu-id="0c008-114">Stream</span></span>          | [<span data-ttu-id="0c008-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0c008-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="0c008-116">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="0c008-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="0c008-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="0c008-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="0c008-118">Stream</span><span class="sxs-lookup"><span data-stu-id="0c008-118">Stream</span></span>          | [<span data-ttu-id="0c008-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="0c008-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="0c008-120">組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。</span><span class="sxs-lookup"><span data-stu-id="0c008-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="0c008-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="0c008-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="0c008-122">ストリーム</span><span class="sxs-lookup"><span data-stu-id="0c008-122">Stream</span></span>          | [<span data-ttu-id="0c008-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="0c008-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="0c008-124">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="0c008-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
