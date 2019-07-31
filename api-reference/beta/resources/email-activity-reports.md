---
title: 電子メール アクティビティ レポート
description: 組織内の電子メールトラフィックの高レベルのビューは、[レポート] ページから入手できます。 また、電子メールアクティビティウィジェットにドリルインして、組織内の電子メールアクティビティのユーザーごとの傾向と詳細を把握することもできます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 2540934b93a1047df5b19c4fe1b477ba30fd798c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972272"
---
# <a name="email-activity-reports"></a><span data-ttu-id="b5b29-104">電子メール アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="b5b29-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5b29-105">組織内の電子メールトラフィックの高レベルのビューは、[レポート] ページから入手できます。</span><span class="sxs-lookup"><span data-stu-id="b5b29-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="b5b29-106">また、電子メールアクティビティウィジェットにドリルインして、組織内の電子メールアクティビティのユーザーごとの傾向と詳細を把握することもできます。</span><span class="sxs-lookup"><span data-stu-id="b5b29-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="b5b29-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5b29-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="b5b29-108">レポート</span><span class="sxs-lookup"><span data-stu-id="b5b29-108">Reports</span></span>

| <span data-ttu-id="b5b29-109">関数</span><span class="sxs-lookup"><span data-stu-id="b5b29-109">Function</span></span>                                 | <span data-ttu-id="b5b29-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b5b29-110">CSV return type</span></span> | <span data-ttu-id="b5b29-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="b5b29-111">JSON return type</span></span>                         | <span data-ttu-id="b5b29-112">説明</span><span class="sxs-lookup"><span data-stu-id="b5b29-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b5b29-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="b5b29-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="b5b29-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b5b29-114">Stream</span></span>          | [<span data-ttu-id="b5b29-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b5b29-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="b5b29-116">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="b5b29-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="b5b29-117">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="b5b29-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="b5b29-118">Stream</span><span class="sxs-lookup"><span data-stu-id="b5b29-118">Stream</span></span>          | [<span data-ttu-id="b5b29-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="b5b29-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="b5b29-120">組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。</span><span class="sxs-lookup"><span data-stu-id="b5b29-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="b5b29-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="b5b29-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="b5b29-122">Stream</span><span class="sxs-lookup"><span data-stu-id="b5b29-122">Stream</span></span>          | [<span data-ttu-id="b5b29-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="b5b29-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="b5b29-124">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="b5b29-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
