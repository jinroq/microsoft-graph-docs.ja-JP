---
title: Office 365 グループ アクティビティ レポート
description: グループ アクティビティ レポートを使用して、組織内の Office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている Office 365 グループの数を確認できます。
localization_priority: Normal
ms.openlocfilehash: c9f7ae5517cf38f3e290db214a6b2f285dce86f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832852"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="9af4d-103">Office 365 グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="9af4d-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="9af4d-104">グループ アクティビティ レポートを使用して、組織内の Office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている Office 365 グループの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="9af4d-104">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="9af4d-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9af4d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="9af4d-106">レポート</span><span class="sxs-lookup"><span data-stu-id="9af4d-106">Reports</span></span>

| <span data-ttu-id="9af4d-107">関数</span><span class="sxs-lookup"><span data-stu-id="9af4d-107">Function</span></span>                                 | <span data-ttu-id="9af4d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9af4d-108">Return Type</span></span> | <span data-ttu-id="9af4d-109">説明</span><span class="sxs-lookup"><span data-stu-id="9af4d-109">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="9af4d-110">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="9af4d-110">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="9af4d-111">Stream</span><span class="sxs-lookup"><span data-stu-id="9af4d-111">Stream</span></span>          | <span data-ttu-id="9af4d-112">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="9af4d-112">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="9af4d-113">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="9af4d-113">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="9af4d-114">Stream</span><span class="sxs-lookup"><span data-stu-id="9af4d-114">Stream</span></span>          | <span data-ttu-id="9af4d-115">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="9af4d-115">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="9af4d-116">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="9af4d-116">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="9af4d-117">Stream</span><span class="sxs-lookup"><span data-stu-id="9af4d-117">Stream</span></span>          | <span data-ttu-id="9af4d-118">グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。</span><span class="sxs-lookup"><span data-stu-id="9af4d-118">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="9af4d-119">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="9af4d-119">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="9af4d-120">Stream</span><span class="sxs-lookup"><span data-stu-id="9af4d-120">Stream</span></span>          | <span data-ttu-id="9af4d-121">すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。</span><span class="sxs-lookup"><span data-stu-id="9af4d-121">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="9af4d-122">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="9af4d-122">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="9af4d-123">Stream</span><span class="sxs-lookup"><span data-stu-id="9af4d-123">Stream</span></span>          | <span data-ttu-id="9af4d-124">Office 365 グループに関連付けられたグループ サイト全体での、ファイルの合計数と、そのうちのアクティブにされたファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="9af4d-124">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
