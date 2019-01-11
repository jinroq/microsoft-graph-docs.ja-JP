---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
localization_priority: Normal
ms.openlocfilehash: e89b5b133b8ebb64a59dfffe75ba9b47d2bf0c7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826160"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="eea39-103">Microsoft Teams デバイスの使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="eea39-103">Microsoft Teams device usage reports</span></span>

> <span data-ttu-id="eea39-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eea39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eea39-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eea39-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="eea39-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eea39-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="eea39-107">マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。</span><span class="sxs-lookup"><span data-stu-id="eea39-107">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="eea39-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="eea39-108">Methods</span></span>

| <span data-ttu-id="eea39-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="eea39-109">Method</span></span>                                   | <span data-ttu-id="eea39-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eea39-110">Return Type</span></span>                              | <span data-ttu-id="eea39-111">説明</span><span class="sxs-lookup"><span data-stu-id="eea39-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="eea39-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="eea39-112">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="eea39-113">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="eea39-113">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="eea39-114">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="eea39-114">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="eea39-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="eea39-115">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="eea39-116">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="eea39-116">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="eea39-117">デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="eea39-117">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="eea39-118">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="eea39-118">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="eea39-119">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="eea39-119">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="eea39-120">デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="eea39-120">Get the number of unique users by device type over the selected time period.</span></span> |
