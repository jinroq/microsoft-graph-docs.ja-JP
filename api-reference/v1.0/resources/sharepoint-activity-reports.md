---
title: SharePoint アクティビティ レポート
description: SharePoint アクティビティ レポートを使用すると、ファイルの操作を参照して、SharePoint のすべてのライセンス ユーザーのアクティビティを取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 5d43f2183c805a29c0bb7a4693a01e14236537d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971894"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="ed751-104">SharePoint アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="ed751-104">SharePoint activity reports</span></span>

<span data-ttu-id="ed751-105">SharePoint アクティビティ レポートを使用すると、ファイルの操作を参照して、SharePoint のすべてのライセンス ユーザーのアクティビティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="ed751-105">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="ed751-106">共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="ed751-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="ed751-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed751-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="ed751-108">レポート</span><span class="sxs-lookup"><span data-stu-id="ed751-108">Reports</span></span>

| <span data-ttu-id="ed751-109">関数</span><span class="sxs-lookup"><span data-stu-id="ed751-109">Function</span></span>                                 | <span data-ttu-id="ed751-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ed751-110">Return Type</span></span> | <span data-ttu-id="ed751-111">説明</span><span class="sxs-lookup"><span data-stu-id="ed751-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="ed751-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="ed751-112">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="ed751-113">Stream</span><span class="sxs-lookup"><span data-stu-id="ed751-113">Stream</span></span>      | <span data-ttu-id="ed751-114">ユーザー別の SharePoint アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed751-114">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="ed751-115">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ed751-115">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="ed751-116">Stream</span><span class="sxs-lookup"><span data-stu-id="ed751-116">Stream</span></span>      | <span data-ttu-id="ed751-117">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed751-117">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="ed751-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ed751-118">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="ed751-119">Stream</span><span class="sxs-lookup"><span data-stu-id="ed751-119">Stream</span></span>      | <span data-ttu-id="ed751-120">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed751-120">Get the trend in the number of active users.</span></span> <span data-ttu-id="ed751-121">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="ed751-121">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="ed751-122">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="ed751-122">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="ed751-123">Stream</span><span class="sxs-lookup"><span data-stu-id="ed751-123">Stream</span></span>      | <span data-ttu-id="ed751-124">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed751-124">Get the number of unique pages visited by users.</span></span> |
