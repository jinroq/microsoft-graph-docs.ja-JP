---
title: Yammer グループ アクティビティ レポート
description: Yammer グループ アクティビティ レポートを使用して、組織内の Yammer グループのアクティビティに関する洞察を得て、作成され、使用されている Yammer グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c5627ea69b34fd186e09b3d381482721a28b09a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033223"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="cce77-103">Yammer グループ アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="cce77-103">Yammer groups activity reports</span></span>

<span data-ttu-id="cce77-104">Yammer グループ アクティビティ レポートを使用して、組織内の Yammer グループのアクティビティに関する洞察を得て、作成され、使用されている Yammer グループの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="cce77-104">You can use the Yammer groups activity reports to gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="cce77-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cce77-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="cce77-106">レポート</span><span class="sxs-lookup"><span data-stu-id="cce77-106">Reports</span></span>

| <span data-ttu-id="cce77-107">関数</span><span class="sxs-lookup"><span data-stu-id="cce77-107">Function</span></span>                                 | <span data-ttu-id="cce77-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cce77-108">Return Type</span></span> | <span data-ttu-id="cce77-109">説明</span><span class="sxs-lookup"><span data-stu-id="cce77-109">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="cce77-110">グループの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="cce77-110">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="cce77-111">Stream</span><span class="sxs-lookup"><span data-stu-id="cce77-111">Stream</span></span>      | <span data-ttu-id="cce77-112">グループ別の Yammer グループ アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="cce77-112">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="cce77-113">グループの数を取得する</span><span class="sxs-lookup"><span data-stu-id="cce77-113">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="cce77-114">Stream</span><span class="sxs-lookup"><span data-stu-id="cce77-114">Stream</span></span>      | <span data-ttu-id="cce77-115">存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。</span><span class="sxs-lookup"><span data-stu-id="cce77-115">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="cce77-116">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="cce77-116">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="cce77-117">Stream</span><span class="sxs-lookup"><span data-stu-id="cce77-117">Stream</span></span>      | <span data-ttu-id="cce77-118">グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="cce77-118">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
