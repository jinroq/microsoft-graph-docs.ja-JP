---
title: Office 365 グループ アクティビティ レポート
description: 組織で Office 365 のグループの活動の洞察を獲得でき、Office 365 のグループの数が表示されるを参照してください作成され、使用されます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 42015937fc13e99373ee0a236f8b20696311028d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520474"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="e6273-103">Office 365 グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="e6273-103">Office 365 Groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6273-104">組織で Office 365 のグループの活動の洞察を獲得でき、Office 365 のグループの数が表示されるを参照してください作成され、使用されます。</span><span class="sxs-lookup"><span data-stu-id="e6273-104">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="e6273-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6273-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="e6273-106">レポート</span><span class="sxs-lookup"><span data-stu-id="e6273-106">Reports</span></span>

| <span data-ttu-id="e6273-107">関数</span><span class="sxs-lookup"><span data-stu-id="e6273-107">Function</span></span>                                 | <span data-ttu-id="e6273-108">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6273-108">CSV return type</span></span> | <span data-ttu-id="e6273-109">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6273-109">JSON return type</span></span>                         | <span data-ttu-id="e6273-110">説明</span><span class="sxs-lookup"><span data-stu-id="e6273-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e6273-111">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="e6273-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="e6273-112">Stream</span><span class="sxs-lookup"><span data-stu-id="e6273-112">Stream</span></span>          | [<span data-ttu-id="e6273-113">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e6273-113">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="e6273-114">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e6273-114">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="e6273-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e6273-115">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="e6273-116">Stream</span><span class="sxs-lookup"><span data-stu-id="e6273-116">Stream</span></span>          | [<span data-ttu-id="e6273-117">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e6273-117">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="e6273-118">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e6273-118">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="e6273-119">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e6273-119">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="e6273-120">Stream</span><span class="sxs-lookup"><span data-stu-id="e6273-120">Stream</span></span>          | [<span data-ttu-id="e6273-121">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="e6273-121">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="e6273-122">グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。</span><span class="sxs-lookup"><span data-stu-id="e6273-122">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="e6273-123">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="e6273-123">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="e6273-124">Stream</span><span class="sxs-lookup"><span data-stu-id="e6273-124">Stream</span></span>          | [<span data-ttu-id="e6273-125">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="e6273-125">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="e6273-126">すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。</span><span class="sxs-lookup"><span data-stu-id="e6273-126">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="e6273-127">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e6273-127">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="e6273-128">Stream</span><span class="sxs-lookup"><span data-stu-id="e6273-128">Stream</span></span>          | [<span data-ttu-id="e6273-129">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="e6273-129">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="e6273-130">Office 365 グループに関連付けられたグループ サイト全体での、ファイルの合計数と、そのうちのアクティブにされたファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e6273-130">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
