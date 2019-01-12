---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2320b997ddc4bb9fb39ef528eecaca8a7c452426
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931033"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="d2597-103">Microsoft Teams デバイスの使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="d2597-103">Microsoft Teams device usage reports</span></span>

> <span data-ttu-id="d2597-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2597-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2597-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2597-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="d2597-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2597-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="d2597-107">マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。</span><span class="sxs-lookup"><span data-stu-id="d2597-107">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="d2597-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2597-108">Methods</span></span>

| <span data-ttu-id="d2597-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2597-109">Method</span></span>                                   | <span data-ttu-id="d2597-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2597-110">Return Type</span></span>                              | <span data-ttu-id="d2597-111">説明</span><span class="sxs-lookup"><span data-stu-id="d2597-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="d2597-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="d2597-112">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="d2597-113">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="d2597-113">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="d2597-114">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2597-114">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="d2597-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="d2597-115">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="d2597-116">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d2597-116">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="d2597-117">デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2597-117">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="d2597-118">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="d2597-118">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="d2597-119">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d2597-119">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="d2597-120">デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2597-120">Get the number of unique users by device type over the selected time period.</span></span> |
