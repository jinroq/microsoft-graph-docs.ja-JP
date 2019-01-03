---
title: SharePoint アクティビティ レポート
description: ファイルとの相互作用を参照して、SharePoint を使用するライセンスを保有するすべてのユーザーの利用状況を取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。
ms.openlocfilehash: fd516b5ca56f8625c98fce943cafc90b32346416
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073319"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="8a091-104">SharePoint アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="8a091-104">SharePoint activity reports</span></span>

> <span data-ttu-id="8a091-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a091-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a091-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a091-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a091-107">ファイルとの相互作用を参照して、SharePoint を使用するライセンスを保有するすべてのユーザーの利用状況を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8a091-107">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="8a091-108">共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="8a091-108">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="8a091-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a091-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="8a091-110">レポート</span><span class="sxs-lookup"><span data-stu-id="8a091-110">Reports</span></span>

| <span data-ttu-id="8a091-111">関数</span><span class="sxs-lookup"><span data-stu-id="8a091-111">Function</span></span>                                 | <span data-ttu-id="8a091-112">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a091-112">CSV Return Type</span></span> | <span data-ttu-id="8a091-113">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a091-113">JSON Return Type</span></span>                         | <span data-ttu-id="8a091-114">説明</span><span class="sxs-lookup"><span data-stu-id="8a091-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="8a091-115">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="8a091-115">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="8a091-116">Stream</span><span class="sxs-lookup"><span data-stu-id="8a091-116">Stream</span></span>          | [<span data-ttu-id="8a091-117">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8a091-117">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="8a091-118">ユーザー別の SharePoint アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a091-118">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="8a091-119">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8a091-119">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="8a091-120">Stream</span><span class="sxs-lookup"><span data-stu-id="8a091-120">Stream</span></span>          | [<span data-ttu-id="8a091-121">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8a091-121">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="8a091-122">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a091-122">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="8a091-123">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8a091-123">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="8a091-124">Stream</span><span class="sxs-lookup"><span data-stu-id="8a091-124">Stream</span></span>          | [<span data-ttu-id="8a091-125">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8a091-125">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="8a091-126">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a091-126">Get the trend in the number of active users.</span></span> <span data-ttu-id="8a091-127">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="8a091-127">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="8a091-128">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="8a091-128">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="8a091-129">Stream</span><span class="sxs-lookup"><span data-stu-id="8a091-129">Stream</span></span>          | [<span data-ttu-id="8a091-130">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="8a091-130">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="8a091-131">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a091-131">Get the number of unique pages visited by users.</span></span> |