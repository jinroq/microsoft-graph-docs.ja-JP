---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 57dcba3a91b15b4980d9e76b7aad6251008f5966
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577432"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="db877-104">Yammer デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="db877-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db877-105">Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="db877-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="db877-106">一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。</span><span class="sxs-lookup"><span data-stu-id="db877-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="db877-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db877-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="db877-108">レポート</span><span class="sxs-lookup"><span data-stu-id="db877-108">Reports</span></span>

| <span data-ttu-id="db877-109">関数</span><span class="sxs-lookup"><span data-stu-id="db877-109">Function</span></span>                                 | <span data-ttu-id="db877-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="db877-110">CSV return type</span></span> | <span data-ttu-id="db877-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="db877-111">JSON return type</span></span>                         | <span data-ttu-id="db877-112">説明</span><span class="sxs-lookup"><span data-stu-id="db877-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="db877-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="db877-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="db877-114">Stream</span><span class="sxs-lookup"><span data-stu-id="db877-114">Stream</span></span>          | [<span data-ttu-id="db877-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="db877-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="db877-116">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="db877-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="db877-117">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="db877-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="db877-118">Stream</span><span class="sxs-lookup"><span data-stu-id="db877-118">Stream</span></span>          | [<span data-ttu-id="db877-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="db877-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="db877-120">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="db877-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="db877-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="db877-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="db877-122">Stream</span><span class="sxs-lookup"><span data-stu-id="db877-122">Stream</span></span>          | [<span data-ttu-id="db877-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="db877-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="db877-124">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="db877-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
