---
title: SharePoint アクティビティ レポート
description: SharePoint アクティビティ レポートを使用すると、ファイルの操作を参照して、SharePoint のすべてのライセンス ユーザーのアクティビティを取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。
localization_priority: Normal
ms.openlocfilehash: 00cc158fee8b5ec108af99c57c089c2259106a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869042"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="13997-104">SharePoint アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="13997-104">SharePoint activity reports</span></span>

<span data-ttu-id="13997-105">SharePoint アクティビティ レポートを使用すると、ファイルの操作を参照して、SharePoint のすべてのライセンス ユーザーのアクティビティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="13997-105">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="13997-106">共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="13997-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="13997-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13997-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="13997-108">レポート</span><span class="sxs-lookup"><span data-stu-id="13997-108">Reports</span></span>

| <span data-ttu-id="13997-109">関数</span><span class="sxs-lookup"><span data-stu-id="13997-109">Function</span></span>                                 | <span data-ttu-id="13997-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="13997-110">Return Type</span></span> | <span data-ttu-id="13997-111">説明</span><span class="sxs-lookup"><span data-stu-id="13997-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="13997-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="13997-112">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="13997-113">Stream</span><span class="sxs-lookup"><span data-stu-id="13997-113">Stream</span></span>      | <span data-ttu-id="13997-114">ユーザー別の SharePoint アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="13997-114">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="13997-115">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="13997-115">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="13997-116">Stream</span><span class="sxs-lookup"><span data-stu-id="13997-116">Stream</span></span>      | <span data-ttu-id="13997-117">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="13997-117">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="13997-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="13997-118">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="13997-119">Stream</span><span class="sxs-lookup"><span data-stu-id="13997-119">Stream</span></span>      | <span data-ttu-id="13997-120">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="13997-120">Get the trend in the number of active users.</span></span> <span data-ttu-id="13997-121">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="13997-121">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="13997-122">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="13997-122">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="13997-123">Stream</span><span class="sxs-lookup"><span data-stu-id="13997-123">Stream</span></span>      | <span data-ttu-id="13997-124">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="13997-124">Get the number of unique pages visited by users.</span></span> |
