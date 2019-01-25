---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f5b24d6d235a8719f5f4b7df0389b5e5971dd8cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521867"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="4f8db-104">Yammer デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="4f8db-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f8db-105">Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="4f8db-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="4f8db-106">一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。</span><span class="sxs-lookup"><span data-stu-id="4f8db-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="4f8db-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f8db-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="4f8db-108">レポート</span><span class="sxs-lookup"><span data-stu-id="4f8db-108">Reports</span></span>

| <span data-ttu-id="4f8db-109">関数</span><span class="sxs-lookup"><span data-stu-id="4f8db-109">Function</span></span>                                 | <span data-ttu-id="4f8db-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4f8db-110">CSV return type</span></span> | <span data-ttu-id="4f8db-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4f8db-111">JSON return type</span></span>                         | <span data-ttu-id="4f8db-112">説明</span><span class="sxs-lookup"><span data-stu-id="4f8db-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4f8db-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="4f8db-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="4f8db-114">Stream</span><span class="sxs-lookup"><span data-stu-id="4f8db-114">Stream</span></span>          | [<span data-ttu-id="4f8db-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="4f8db-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="4f8db-116">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="4f8db-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="4f8db-117">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="4f8db-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="4f8db-118">Stream</span><span class="sxs-lookup"><span data-stu-id="4f8db-118">Stream</span></span>          | [<span data-ttu-id="4f8db-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f8db-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="4f8db-120">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="4f8db-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="4f8db-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="4f8db-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="4f8db-122">Stream</span><span class="sxs-lookup"><span data-stu-id="4f8db-122">Stream</span></span>          | [<span data-ttu-id="4f8db-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f8db-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="4f8db-124">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="4f8db-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
