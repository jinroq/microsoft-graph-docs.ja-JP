---
title: Yammer グループ アクティビティ レポート
description: Yammer グループ アクティビティ レポートを使用して、組織内の Yammer グループのアクティビティに関する洞察を得て、作成され、使用されている Yammer グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fd29d0ed2e1bc551595c8b8403325f64fc44998d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571010"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="94777-103">Yammer グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="94777-103">Yammer groups activity reports</span></span>

<span data-ttu-id="94777-104">Yammer グループ アクティビティ レポートを使用して、組織内の Yammer グループのアクティビティに関する洞察を得て、作成され、使用されている Yammer グループの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="94777-104">You can use the Yammer groups activity reports to gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="94777-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94777-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="94777-106">レポート</span><span class="sxs-lookup"><span data-stu-id="94777-106">Reports</span></span>

| <span data-ttu-id="94777-107">関数</span><span class="sxs-lookup"><span data-stu-id="94777-107">Function</span></span>                                 | <span data-ttu-id="94777-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="94777-108">Return Type</span></span> | <span data-ttu-id="94777-109">説明</span><span class="sxs-lookup"><span data-stu-id="94777-109">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="94777-110">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="94777-110">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="94777-111">Stream</span><span class="sxs-lookup"><span data-stu-id="94777-111">Stream</span></span>      | <span data-ttu-id="94777-112">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="94777-112">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="94777-113">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="94777-113">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="94777-114">Stream</span><span class="sxs-lookup"><span data-stu-id="94777-114">Stream</span></span>      | <span data-ttu-id="94777-115">存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。</span><span class="sxs-lookup"><span data-stu-id="94777-115">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="94777-116">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="94777-116">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="94777-117">Stream</span><span class="sxs-lookup"><span data-stu-id="94777-117">Stream</span></span>      | <span data-ttu-id="94777-118">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="94777-118">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
