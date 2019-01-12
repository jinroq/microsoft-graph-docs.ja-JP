---
title: 電子メール アクティビティ レポート
description: '[レポート] ページから、組織内で電子メール トラフィックの高レベルのビューを取得できます。 傾向と、組織内の電子メール活動のユーザーごとの詳細を理解する電子メール活動のウィジェットにドリルダウンすることもできます。'
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: ccbe53a783da8f45294c3140f6cbf9405d1d1f04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947681"
---
# <a name="email-activity-reports"></a><span data-ttu-id="8904a-104">電子メール アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="8904a-104">Email activity reports</span></span>

> <span data-ttu-id="8904a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8904a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8904a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8904a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8904a-107">[レポート] ページから、組織内で電子メール トラフィックの高レベルのビューを取得できます。</span><span class="sxs-lookup"><span data-stu-id="8904a-107">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="8904a-108">傾向と、組織内の電子メール活動のユーザーごとの詳細を理解する電子メール活動のウィジェットにドリルダウンすることもできます。</span><span class="sxs-lookup"><span data-stu-id="8904a-108">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="8904a-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8904a-109">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="8904a-110">レポート</span><span class="sxs-lookup"><span data-stu-id="8904a-110">Reports</span></span>

| <span data-ttu-id="8904a-111">関数</span><span class="sxs-lookup"><span data-stu-id="8904a-111">Function</span></span>                                 | <span data-ttu-id="8904a-112">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8904a-112">CSV return type</span></span> | <span data-ttu-id="8904a-113">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8904a-113">JSON return type</span></span>                         | <span data-ttu-id="8904a-114">説明</span><span class="sxs-lookup"><span data-stu-id="8904a-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="8904a-115">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="8904a-115">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="8904a-116">Stream</span><span class="sxs-lookup"><span data-stu-id="8904a-116">Stream</span></span>          | [<span data-ttu-id="8904a-117">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8904a-117">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="8904a-118">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8904a-118">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="8904a-119">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8904a-119">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="8904a-120">Stream</span><span class="sxs-lookup"><span data-stu-id="8904a-120">Stream</span></span>          | [<span data-ttu-id="8904a-121">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8904a-121">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="8904a-122">組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。</span><span class="sxs-lookup"><span data-stu-id="8904a-122">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="8904a-123">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8904a-123">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="8904a-124">Stream</span><span class="sxs-lookup"><span data-stu-id="8904a-124">Stream</span></span>          | [<span data-ttu-id="8904a-125">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8904a-125">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="8904a-126">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="8904a-126">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
