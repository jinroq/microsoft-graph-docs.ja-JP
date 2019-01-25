---
title: Yammer グループ アクティビティ レポート
description: 組織で Yammer グループの活動の洞察を獲得でき、Yammer グループの数が表示されるを参照してください作成され、使用されます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 05e5826a85e7d2e37af82cdf6277857746b1b922
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514160"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="6e5eb-103">Yammer グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="6e5eb-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e5eb-104">組織で Yammer グループの活動の洞察を獲得でき、Yammer グループの数が表示されるを参照してください作成され、使用されます。</span><span class="sxs-lookup"><span data-stu-id="6e5eb-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="6e5eb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e5eb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="6e5eb-106">レポート</span><span class="sxs-lookup"><span data-stu-id="6e5eb-106">Reports</span></span>

| <span data-ttu-id="6e5eb-107">関数</span><span class="sxs-lookup"><span data-stu-id="6e5eb-107">Function</span></span>                                 | <span data-ttu-id="6e5eb-108">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6e5eb-108">CSV return type</span></span> | <span data-ttu-id="6e5eb-109">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6e5eb-109">JSON return type</span></span>                         | <span data-ttu-id="6e5eb-110">説明</span><span class="sxs-lookup"><span data-stu-id="6e5eb-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6e5eb-111">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="6e5eb-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="6e5eb-112">Stream</span><span class="sxs-lookup"><span data-stu-id="6e5eb-112">Stream</span></span>          | [<span data-ttu-id="6e5eb-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="6e5eb-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="6e5eb-114">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e5eb-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="6e5eb-115">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="6e5eb-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="6e5eb-116">Stream</span><span class="sxs-lookup"><span data-stu-id="6e5eb-116">Stream</span></span>          | [<span data-ttu-id="6e5eb-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="6e5eb-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="6e5eb-118">存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e5eb-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="6e5eb-119">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="6e5eb-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="6e5eb-120">Stream</span><span class="sxs-lookup"><span data-stu-id="6e5eb-120">Stream</span></span>          | [<span data-ttu-id="6e5eb-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6e5eb-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="6e5eb-122">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e5eb-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
