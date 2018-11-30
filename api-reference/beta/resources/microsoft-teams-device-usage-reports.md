---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
ms.openlocfilehash: 22476c0891111d5f160e528477aab78ca5cc2e90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067263"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="c81b9-103">Microsoft Teams デバイスの使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="c81b9-103">Microsoft Teams device usage reports</span></span>

> <span data-ttu-id="c81b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c81b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c81b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c81b9-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="c81b9-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c81b9-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="c81b9-107">マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。</span><span class="sxs-lookup"><span data-stu-id="c81b9-107">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="c81b9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c81b9-108">Methods</span></span>

| <span data-ttu-id="c81b9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c81b9-109">Method</span></span>                                   | <span data-ttu-id="c81b9-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c81b9-110">Return Type</span></span>                              | <span data-ttu-id="c81b9-111">説明</span><span class="sxs-lookup"><span data-stu-id="c81b9-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="c81b9-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="c81b9-112">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="c81b9-113">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="c81b9-113">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="c81b9-114">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c81b9-114">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="c81b9-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c81b9-115">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="c81b9-116">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="c81b9-116">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="c81b9-117">デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c81b9-117">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="c81b9-118">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c81b9-118">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="c81b9-119">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="c81b9-119">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="c81b9-120">デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c81b9-120">Get the number of unique users by device type over the selected time period.</span></span> |
