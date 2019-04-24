---
title: OneDrive 使用状況レポート
description: 組織内のすべての onedrive アカウントで使用されているファイルと記憶域の合計数に関して、onedrive から取得した値の概要を把握することができます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 また、OneDrive アカウントの詳細についても説明します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1f899c3a60e1c0d66dd3b7e075bf0daf13de0b43
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457089"
---
# <a name="onedrive-usage-reports"></a><span data-ttu-id="d842e-105">OneDrive 使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="d842e-105">OneDrive usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d842e-106">組織内のすべての onedrive アカウントで使用されているファイルと記憶域の合計数に関して、onedrive から取得した値の概要を把握することができます。</span><span class="sxs-lookup"><span data-stu-id="d842e-106">You can get a high-level view of the value you are getting from OneDrive in terms of the total number of files and storage used across all the OneDrive accounts in your organization.</span></span> <span data-ttu-id="d842e-107">さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="d842e-107">You can then drill down to understand the trends of active OneDrive accounts, how many files users have interacted with, and how much storage is used.</span></span> <span data-ttu-id="d842e-108">また、OneDrive アカウントの詳細についても説明します。</span><span class="sxs-lookup"><span data-stu-id="d842e-108">It also gives you the per OneDrive account details.</span></span>

> <span data-ttu-id="d842e-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d842e-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="reports"></a><span data-ttu-id="d842e-110">レポート</span><span class="sxs-lookup"><span data-stu-id="d842e-110">Reports</span></span>

| <span data-ttu-id="d842e-111">関数</span><span class="sxs-lookup"><span data-stu-id="d842e-111">Function</span></span>                                 | <span data-ttu-id="d842e-112">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d842e-112">CSV return type</span></span> | <span data-ttu-id="d842e-113">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="d842e-113">JSON return type</span></span>                         | <span data-ttu-id="d842e-114">説明</span><span class="sxs-lookup"><span data-stu-id="d842e-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d842e-115">アカウントの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="d842e-115">Get account detail</span></span>](../api/reportroot-getonedriveusageaccountdetail.md) | <span data-ttu-id="d842e-116">Stream</span><span class="sxs-lookup"><span data-stu-id="d842e-116">Stream</span></span>          | [<span data-ttu-id="d842e-117">onedrive のアカウントの詳細</span><span class="sxs-lookup"><span data-stu-id="d842e-117">oneDriveUsageAccountDetail</span></span>](../resources/onedriveusageaccountdetail.md) | <span data-ttu-id="d842e-118">アカウント別の OneDrive の使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d842e-118">Get details about OneDrive usage by account.</span></span> |
| [<span data-ttu-id="d842e-119">アカウントの数を取得する</span><span class="sxs-lookup"><span data-stu-id="d842e-119">Get account counts</span></span>](../api/reportroot-getonedriveusageaccountcounts.md) | <span data-ttu-id="d842e-120">Stream</span><span class="sxs-lookup"><span data-stu-id="d842e-120">Stream</span></span>          | [<span data-ttu-id="d842e-121">onedrive のアカウント数</span><span class="sxs-lookup"><span data-stu-id="d842e-121">oneDriveUsageAccountCounts</span></span>](../resources/onedriveusageaccountcounts.md) | <span data-ttu-id="d842e-122">アクティブな OneDrive for Business サイトの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="d842e-122">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="d842e-123">ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。</span><span class="sxs-lookup"><span data-stu-id="d842e-123">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span> |
| [<span data-ttu-id="d842e-124">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="d842e-124">Get file counts</span></span>](../api/reportroot-getonedriveusagefilecounts.md) | <span data-ttu-id="d842e-125">Stream</span><span class="sxs-lookup"><span data-stu-id="d842e-125">Stream</span></span>          | [<span data-ttu-id="d842e-126">oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="d842e-126">oneDriveUsageFileCounts</span></span>](../resources/onedriveusagefilecounts.md) | <span data-ttu-id="d842e-127">すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="d842e-127">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="d842e-128">ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="d842e-128">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span> |
| [<span data-ttu-id="d842e-129">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="d842e-129">Get storage</span></span>](../api/reportroot-getonedriveusagestorage.md) | <span data-ttu-id="d842e-130">Stream</span><span class="sxs-lookup"><span data-stu-id="d842e-130">Stream</span></span>          | [<span data-ttu-id="d842e-131">サイトの保存場所</span><span class="sxs-lookup"><span data-stu-id="d842e-131">siteUsageStorage</span></span>](../resources/siteusagestorage.md) | <span data-ttu-id="d842e-132">OneDrive for Business で使用しているストレージの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="d842e-132">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
