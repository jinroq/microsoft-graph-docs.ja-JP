---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f36ed78805bc664adfbbd4ced9bc86b1444ab262
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007005"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="eb13a-104">Yammer デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="eb13a-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb13a-105">Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="eb13a-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="eb13a-106">一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。</span><span class="sxs-lookup"><span data-stu-id="eb13a-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="eb13a-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb13a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="eb13a-108">レポート</span><span class="sxs-lookup"><span data-stu-id="eb13a-108">Reports</span></span>

| <span data-ttu-id="eb13a-109">関数</span><span class="sxs-lookup"><span data-stu-id="eb13a-109">Function</span></span>                                 | <span data-ttu-id="eb13a-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eb13a-110">CSV return type</span></span> | <span data-ttu-id="eb13a-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="eb13a-111">JSON return type</span></span>                         | <span data-ttu-id="eb13a-112">説明</span><span class="sxs-lookup"><span data-stu-id="eb13a-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="eb13a-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="eb13a-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="eb13a-114">Stream</span><span class="sxs-lookup"><span data-stu-id="eb13a-114">Stream</span></span>          | [<span data-ttu-id="eb13a-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="eb13a-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="eb13a-116">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="eb13a-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="eb13a-117">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="eb13a-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="eb13a-118">Stream</span><span class="sxs-lookup"><span data-stu-id="eb13a-118">Stream</span></span>          | [<span data-ttu-id="eb13a-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="eb13a-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="eb13a-120">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="eb13a-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="eb13a-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="eb13a-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="eb13a-122">Stream</span><span class="sxs-lookup"><span data-stu-id="eb13a-122">Stream</span></span>          | [<span data-ttu-id="eb13a-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="eb13a-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="eb13a-124">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="eb13a-124">Get the number of daily users by device type.</span></span> |
