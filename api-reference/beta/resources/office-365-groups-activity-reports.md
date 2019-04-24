---
title: Office 365 グループ アクティビティ レポート
description: 組織内の office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている office 365 グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e698a1096d244b864bbb15cf06c16e8cf79ff1f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505577"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="bf48f-103">Office 365 グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="bf48f-103">Office 365 Groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf48f-104">組織内の office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている office 365 グループの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="bf48f-104">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="bf48f-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf48f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="bf48f-106">レポート</span><span class="sxs-lookup"><span data-stu-id="bf48f-106">Reports</span></span>

| <span data-ttu-id="bf48f-107">関数</span><span class="sxs-lookup"><span data-stu-id="bf48f-107">Function</span></span>                                 | <span data-ttu-id="bf48f-108">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bf48f-108">CSV return type</span></span> | <span data-ttu-id="bf48f-109">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="bf48f-109">JSON return type</span></span>                         | <span data-ttu-id="bf48f-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf48f-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="bf48f-111">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="bf48f-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="bf48f-112">Stream</span><span class="sxs-lookup"><span data-stu-id="bf48f-112">Stream</span></span>          | [<span data-ttu-id="bf48f-113">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bf48f-113">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="bf48f-114">グループ別の Office 365 グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf48f-114">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="bf48f-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="bf48f-115">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="bf48f-116">ストリーム</span><span class="sxs-lookup"><span data-stu-id="bf48f-116">Stream</span></span>          | [<span data-ttu-id="bf48f-117">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="bf48f-117">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="bf48f-118">グループ ワークロード全体のグループ活動の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf48f-118">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="bf48f-119">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="bf48f-119">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="bf48f-120">Stream</span><span class="sxs-lookup"><span data-stu-id="bf48f-120">Stream</span></span>          | [<span data-ttu-id="bf48f-121">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="bf48f-121">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="bf48f-122">グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。</span><span class="sxs-lookup"><span data-stu-id="bf48f-122">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="bf48f-123">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="bf48f-123">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="bf48f-124">Stream</span><span class="sxs-lookup"><span data-stu-id="bf48f-124">Stream</span></span>          | [<span data-ttu-id="bf48f-125">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="bf48f-125">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="bf48f-126">すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf48f-126">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="bf48f-127">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="bf48f-127">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="bf48f-128">Stream</span><span class="sxs-lookup"><span data-stu-id="bf48f-128">Stream</span></span>          | [<span data-ttu-id="bf48f-129">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="bf48f-129">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="bf48f-130">Office 365 グループに関連付けられたグループ サイト全体での、ファイルの合計数と、そのうちのアクティブにされたファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf48f-130">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
