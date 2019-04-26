---
title: 電子メール アクティビティ レポート
description: 組織内の電子メールトラフィックの高レベルのビューは、[レポート] ページから入手できます。 また、電子メールアクティビティウィジェットにドリルインして、組織内の電子メールアクティビティのユーザーごとの傾向と詳細を把握することもできます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: d3adb15bd6bb6c60b3957cd81b5d2f915ecfaa8c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333929"
---
# <a name="email-activity-reports"></a><span data-ttu-id="14a85-104">電子メール アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="14a85-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14a85-105">組織内の電子メールトラフィックの高レベルのビューは、[レポート] ページから入手できます。</span><span class="sxs-lookup"><span data-stu-id="14a85-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="14a85-106">また、電子メールアクティビティウィジェットにドリルインして、組織内の電子メールアクティビティのユーザーごとの傾向と詳細を把握することもできます。</span><span class="sxs-lookup"><span data-stu-id="14a85-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="14a85-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14a85-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="14a85-108">レポート</span><span class="sxs-lookup"><span data-stu-id="14a85-108">Reports</span></span>

| <span data-ttu-id="14a85-109">関数</span><span class="sxs-lookup"><span data-stu-id="14a85-109">Function</span></span>                                 | <span data-ttu-id="14a85-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14a85-110">CSV return type</span></span> | <span data-ttu-id="14a85-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="14a85-111">JSON return type</span></span>                         | <span data-ttu-id="14a85-112">説明</span><span class="sxs-lookup"><span data-stu-id="14a85-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="14a85-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="14a85-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="14a85-114">Stream</span><span class="sxs-lookup"><span data-stu-id="14a85-114">Stream</span></span>          | [<span data-ttu-id="14a85-115">emailactivityuserdetail</span><span class="sxs-lookup"><span data-stu-id="14a85-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="14a85-116">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="14a85-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="14a85-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="14a85-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="14a85-118">Stream</span><span class="sxs-lookup"><span data-stu-id="14a85-118">Stream</span></span>          | [<span data-ttu-id="14a85-119">emailactivitysummary</span><span class="sxs-lookup"><span data-stu-id="14a85-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="14a85-120">組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。</span><span class="sxs-lookup"><span data-stu-id="14a85-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="14a85-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="14a85-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="14a85-122">Stream</span><span class="sxs-lookup"><span data-stu-id="14a85-122">Stream</span></span>          | [<span data-ttu-id="14a85-123">emailactivitysummary</span><span class="sxs-lookup"><span data-stu-id="14a85-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="14a85-124">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="14a85-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
