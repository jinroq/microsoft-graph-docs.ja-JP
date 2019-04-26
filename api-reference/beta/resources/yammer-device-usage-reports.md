---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2c253d58d3f8b0bdd07d902bbcbe77af6a1666e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342789"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="ce009-104">Yammer デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="ce009-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce009-105">Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="ce009-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="ce009-106">一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。</span><span class="sxs-lookup"><span data-stu-id="ce009-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="ce009-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce009-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="ce009-108">レポート</span><span class="sxs-lookup"><span data-stu-id="ce009-108">Reports</span></span>

| <span data-ttu-id="ce009-109">関数</span><span class="sxs-lookup"><span data-stu-id="ce009-109">Function</span></span>                                 | <span data-ttu-id="ce009-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce009-110">CSV return type</span></span> | <span data-ttu-id="ce009-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="ce009-111">JSON return type</span></span>                         | <span data-ttu-id="ce009-112">説明</span><span class="sxs-lookup"><span data-stu-id="ce009-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ce009-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="ce009-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="ce009-114">Stream</span><span class="sxs-lookup"><span data-stu-id="ce009-114">Stream</span></span>          | [<span data-ttu-id="ce009-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ce009-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="ce009-116">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce009-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="ce009-117">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ce009-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="ce009-118">Stream</span><span class="sxs-lookup"><span data-stu-id="ce009-118">Stream</span></span>          | [<span data-ttu-id="ce009-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ce009-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="ce009-120">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce009-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="ce009-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ce009-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="ce009-122">Stream</span><span class="sxs-lookup"><span data-stu-id="ce009-122">Stream</span></span>          | [<span data-ttu-id="ce009-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ce009-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="ce009-124">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce009-124">Get the number of daily users by device type.</span></span> |
