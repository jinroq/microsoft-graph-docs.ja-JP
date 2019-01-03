---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
ms.openlocfilehash: da94fb91d3feb17052cf02b09e27cdc70b7f734b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072470"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="465bc-104">Yammer デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="465bc-104">Yammer device usage reports</span></span>

> <span data-ttu-id="465bc-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="465bc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="465bc-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="465bc-106">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="465bc-107">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="465bc-107">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="465bc-108">Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="465bc-108">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="465bc-109">一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。</span><span class="sxs-lookup"><span data-stu-id="465bc-109">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="465bc-110">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="465bc-110">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="465bc-111">レポート</span><span class="sxs-lookup"><span data-stu-id="465bc-111">Reports</span></span>

| <span data-ttu-id="465bc-112">関数</span><span class="sxs-lookup"><span data-stu-id="465bc-112">Function</span></span>                                 | <span data-ttu-id="465bc-113">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="465bc-113">CSV return type</span></span> | <span data-ttu-id="465bc-114">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="465bc-114">JSON return type</span></span>                         | <span data-ttu-id="465bc-115">説明</span><span class="sxs-lookup"><span data-stu-id="465bc-115">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="465bc-116">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="465bc-116">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="465bc-117">Stream</span><span class="sxs-lookup"><span data-stu-id="465bc-117">Stream</span></span>          | [<span data-ttu-id="465bc-118">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="465bc-118">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="465bc-119">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="465bc-119">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="465bc-120">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="465bc-120">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="465bc-121">Stream</span><span class="sxs-lookup"><span data-stu-id="465bc-121">Stream</span></span>          | [<span data-ttu-id="465bc-122">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="465bc-122">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="465bc-123">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="465bc-123">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="465bc-124">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="465bc-124">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="465bc-125">Stream</span><span class="sxs-lookup"><span data-stu-id="465bc-125">Stream</span></span>          | [<span data-ttu-id="465bc-126">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="465bc-126">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="465bc-127">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="465bc-127">Get the number of daily users by device type.</span></span> |