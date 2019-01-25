---
title: SharePoint アクティビティ レポート
description: ファイルとの相互作用を参照して、SharePoint を使用するライセンスを保有するすべてのユーザーの利用状況を取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 55013b3ada74e876734a83acf512a532e32cc4be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522197"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="cb0cd-104">SharePoint アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="cb0cd-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb0cd-105">ファイルとの相互作用を参照して、SharePoint を使用するライセンスを保有するすべてのユーザーの利用状況を取得できます。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="cb0cd-106">共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="cb0cd-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="cb0cd-108">レポート</span><span class="sxs-lookup"><span data-stu-id="cb0cd-108">Reports</span></span>

| <span data-ttu-id="cb0cd-109">関数</span><span class="sxs-lookup"><span data-stu-id="cb0cd-109">Function</span></span>                                 | <span data-ttu-id="cb0cd-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cb0cd-110">CSV Return Type</span></span> | <span data-ttu-id="cb0cd-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cb0cd-111">JSON Return Type</span></span>                         | <span data-ttu-id="cb0cd-112">説明</span><span class="sxs-lookup"><span data-stu-id="cb0cd-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="cb0cd-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="cb0cd-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="cb0cd-114">Stream</span><span class="sxs-lookup"><span data-stu-id="cb0cd-114">Stream</span></span>          | [<span data-ttu-id="cb0cd-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="cb0cd-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="cb0cd-116">ユーザー別の SharePoint アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="cb0cd-117">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="cb0cd-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="cb0cd-118">Stream</span><span class="sxs-lookup"><span data-stu-id="cb0cd-118">Stream</span></span>          | [<span data-ttu-id="cb0cd-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="cb0cd-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="cb0cd-120">SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="cb0cd-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="cb0cd-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="cb0cd-122">Stream</span><span class="sxs-lookup"><span data-stu-id="cb0cd-122">Stream</span></span>          | [<span data-ttu-id="cb0cd-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cb0cd-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="cb0cd-124">アクティブ ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="cb0cd-125">ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="cb0cd-126">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="cb0cd-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="cb0cd-127">Stream</span><span class="sxs-lookup"><span data-stu-id="cb0cd-127">Stream</span></span>          | [<span data-ttu-id="cb0cd-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="cb0cd-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="cb0cd-129">ユーザーがアクセスしたそれぞれ別個のページ数を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb0cd-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
