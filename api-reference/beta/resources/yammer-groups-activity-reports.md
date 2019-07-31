---
title: Yammer グループ アクティビティ レポート
description: 組織内の Yammer グループのアクティビティについての洞察を得て、作成され、使用されている Yammer グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 07a78a4b2047e03beee611443240f56739f76b4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963842"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="e4970-103">Yammer グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="e4970-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4970-104">組織内の Yammer グループのアクティビティについての洞察を得て、作成され、使用されている Yammer グループの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="e4970-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="e4970-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4970-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="e4970-106">レポート</span><span class="sxs-lookup"><span data-stu-id="e4970-106">Reports</span></span>

| <span data-ttu-id="e4970-107">関数</span><span class="sxs-lookup"><span data-stu-id="e4970-107">Function</span></span>                                 | <span data-ttu-id="e4970-108">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e4970-108">CSV return type</span></span> | <span data-ttu-id="e4970-109">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="e4970-109">JSON return type</span></span>                         | <span data-ttu-id="e4970-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4970-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e4970-111">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="e4970-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="e4970-112">Stream</span><span class="sxs-lookup"><span data-stu-id="e4970-112">Stream</span></span>          | [<span data-ttu-id="e4970-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e4970-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="e4970-114">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e4970-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="e4970-115">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e4970-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="e4970-116">Stream</span><span class="sxs-lookup"><span data-stu-id="e4970-116">Stream</span></span>          | [<span data-ttu-id="e4970-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="e4970-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="e4970-118">存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e4970-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="e4970-119">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e4970-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="e4970-120">Stream</span><span class="sxs-lookup"><span data-stu-id="e4970-120">Stream</span></span>          | [<span data-ttu-id="e4970-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e4970-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="e4970-122">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e4970-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
