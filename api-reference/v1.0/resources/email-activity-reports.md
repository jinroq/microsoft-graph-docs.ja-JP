---
title: 電子メール アクティビティ レポート
description: 電子メール アクティビティ レポートを使用して、組織内の電子メール トラフィックの詳細ビューを取得します。 [メール アクティビティ] ウィジェットに進み、組織内のユーザーごとの電子メール アクティビティの傾向と詳細を把握することもできます。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: e28e968a536b4025094ba0376973352f7d9cc949
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981785"
---
# <a name="email-activity-reports"></a><span data-ttu-id="71e02-104">電子メール アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="71e02-104">Email activity reports</span></span>

<span data-ttu-id="71e02-105">電子メール アクティビティ レポートを使用して、組織内の電子メール トラフィックの詳細ビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="71e02-105">Use the email activity reports to get a high level view of email traffic within your organization.</span></span> <span data-ttu-id="71e02-106">[メール アクティビティ] ウィジェットに進み、組織内のユーザーごとの電子メール アクティビティの傾向と詳細を把握することもできます。</span><span class="sxs-lookup"><span data-stu-id="71e02-106">You can also drill into the Email Activity widget to understand the trends and details of the email activity per user in your organization.</span></span>

> <span data-ttu-id="71e02-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71e02-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="71e02-108">レポート</span><span class="sxs-lookup"><span data-stu-id="71e02-108">Reports</span></span>

| <span data-ttu-id="71e02-109">関数</span><span class="sxs-lookup"><span data-stu-id="71e02-109">Function</span></span>                                 | <span data-ttu-id="71e02-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="71e02-110">Return Type</span></span> | <span data-ttu-id="71e02-111">説明</span><span class="sxs-lookup"><span data-stu-id="71e02-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="71e02-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="71e02-112">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="71e02-113">Stream</span><span class="sxs-lookup"><span data-stu-id="71e02-113">Stream</span></span>      | <span data-ttu-id="71e02-114">ユーザーが実行した電子メール アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="71e02-114">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="71e02-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="71e02-115">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="71e02-116">Stream</span><span class="sxs-lookup"><span data-stu-id="71e02-116">Stream</span></span>      | <span data-ttu-id="71e02-117">組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。</span><span class="sxs-lookup"><span data-stu-id="71e02-117">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="71e02-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="71e02-118">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="71e02-119">Stream</span><span class="sxs-lookup"><span data-stu-id="71e02-119">Stream</span></span>      | <span data-ttu-id="71e02-120">送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="71e02-120">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
