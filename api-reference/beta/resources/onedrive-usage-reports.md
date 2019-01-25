---
title: OneDrive 使用状況レポート
description: OneDrive ファイルと OneDrive のすべてのアカウントが組織内で使用されているストレージの合計数から取得する値の高度なビューを取得できます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 できます、単位の OneDrive のアカウントの詳細。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c5a73b33f4422440df8817c3f6a69299eedeae50
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519837"
---
# <a name="onedrive-usage-reports"></a><span data-ttu-id="64652-105">OneDrive 使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="64652-105">OneDrive usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64652-106">OneDrive ファイルと OneDrive のすべてのアカウントが組織内で使用されているストレージの合計数から取得する値の高度なビューを取得できます。</span><span class="sxs-lookup"><span data-stu-id="64652-106">You can get a high-level view of the value you are getting from OneDrive in terms of the total number of files and storage used across all the OneDrive accounts in your organization.</span></span> <span data-ttu-id="64652-107">さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="64652-107">You can then drill down to understand the trends of active OneDrive accounts, how many files users have interacted with, and how much storage is used.</span></span> <span data-ttu-id="64652-108">できます、単位の OneDrive のアカウントの詳細。</span><span class="sxs-lookup"><span data-stu-id="64652-108">It also gives you the per OneDrive account details.</span></span>

> <span data-ttu-id="64652-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64652-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="reports"></a><span data-ttu-id="64652-110">レポート</span><span class="sxs-lookup"><span data-stu-id="64652-110">Reports</span></span>

| <span data-ttu-id="64652-111">関数</span><span class="sxs-lookup"><span data-stu-id="64652-111">Function</span></span>                                 | <span data-ttu-id="64652-112">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64652-112">CSV return type</span></span> | <span data-ttu-id="64652-113">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64652-113">JSON return type</span></span>                         | <span data-ttu-id="64652-114">説明</span><span class="sxs-lookup"><span data-stu-id="64652-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="64652-115">アカウントの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="64652-115">Get account detail</span></span>](../api/reportroot-getonedriveusageaccountdetail.md) | <span data-ttu-id="64652-116">Stream</span><span class="sxs-lookup"><span data-stu-id="64652-116">Stream</span></span>          | [<span data-ttu-id="64652-117">oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="64652-117">oneDriveUsageAccountDetail</span></span>](../resources/onedriveusageaccountdetail.md) | <span data-ttu-id="64652-118">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="64652-118">Get details about OneDrive usage by account.</span></span> |
| [<span data-ttu-id="64652-119">アカウントの数を取得する</span><span class="sxs-lookup"><span data-stu-id="64652-119">Get account counts</span></span>](../api/reportroot-getonedriveusageaccountcounts.md) | <span data-ttu-id="64652-120">Stream</span><span class="sxs-lookup"><span data-stu-id="64652-120">Stream</span></span>          | [<span data-ttu-id="64652-121">oneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="64652-121">oneDriveUsageAccountCounts</span></span>](../resources/onedriveusageaccountcounts.md) | <span data-ttu-id="64652-122">アクティブな OneDrive for Business サイトの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="64652-122">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="64652-123">ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。</span><span class="sxs-lookup"><span data-stu-id="64652-123">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span> |
| [<span data-ttu-id="64652-124">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="64652-124">Get file counts</span></span>](../api/reportroot-getonedriveusagefilecounts.md) | <span data-ttu-id="64652-125">Stream</span><span class="sxs-lookup"><span data-stu-id="64652-125">Stream</span></span>          | [<span data-ttu-id="64652-126">oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="64652-126">oneDriveUsageFileCounts</span></span>](../resources/onedriveusagefilecounts.md) | <span data-ttu-id="64652-127">すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="64652-127">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="64652-128">ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="64652-128">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="64652-129">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="64652-129">Get storage</span></span>](../api/reportroot-getonedriveusagestorage.md) | <span data-ttu-id="64652-130">Stream</span><span class="sxs-lookup"><span data-stu-id="64652-130">Stream</span></span>          | [<span data-ttu-id="64652-131">siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="64652-131">siteUsageStorage</span></span>](../resources/siteusagestorage.md) | <span data-ttu-id="64652-132">OneDrive for Business で使用しているストレージの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="64652-132">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
