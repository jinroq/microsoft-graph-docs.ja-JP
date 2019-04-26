---
title: Yammer グループ アクティビティ レポート
description: 組織内の yammer グループのアクティビティについての洞察を得て、作成され、使用されている yammer グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9035984cf33c56811dc411a6c9cc01e6d438d194
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342794"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="876fb-103">Yammer グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="876fb-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="876fb-104">組織内の yammer グループのアクティビティについての洞察を得て、作成され、使用されている yammer グループの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="876fb-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="876fb-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="876fb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="876fb-106">レポート</span><span class="sxs-lookup"><span data-stu-id="876fb-106">Reports</span></span>

| <span data-ttu-id="876fb-107">関数</span><span class="sxs-lookup"><span data-stu-id="876fb-107">Function</span></span>                                 | <span data-ttu-id="876fb-108">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="876fb-108">CSV return type</span></span> | <span data-ttu-id="876fb-109">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="876fb-109">JSON return type</span></span>                         | <span data-ttu-id="876fb-110">説明</span><span class="sxs-lookup"><span data-stu-id="876fb-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="876fb-111">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="876fb-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="876fb-112">Stream</span><span class="sxs-lookup"><span data-stu-id="876fb-112">Stream</span></span>          | [<span data-ttu-id="876fb-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="876fb-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="876fb-114">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="876fb-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="876fb-115">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="876fb-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="876fb-116">Stream</span><span class="sxs-lookup"><span data-stu-id="876fb-116">Stream</span></span>          | [<span data-ttu-id="876fb-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="876fb-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="876fb-118">存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。</span><span class="sxs-lookup"><span data-stu-id="876fb-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="876fb-119">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="876fb-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="876fb-120">Stream</span><span class="sxs-lookup"><span data-stu-id="876fb-120">Stream</span></span>          | [<span data-ttu-id="876fb-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="876fb-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="876fb-122">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="876fb-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
