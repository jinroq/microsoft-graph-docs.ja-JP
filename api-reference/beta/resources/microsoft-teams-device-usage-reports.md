---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d19df5132a67ac5862535a329eadbdff7044798c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576641"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="b2a3b-103">Microsoft Teams デバイスの使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="b2a3b-103">Microsoft Teams device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2a3b-104">マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-104">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="b2a3b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2a3b-105">Methods</span></span>

| <span data-ttu-id="b2a3b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2a3b-106">Method</span></span>                                   | <span data-ttu-id="b2a3b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b2a3b-107">Return Type</span></span>                              | <span data-ttu-id="b2a3b-108">説明</span><span class="sxs-lookup"><span data-stu-id="b2a3b-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="b2a3b-109">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="b2a3b-109">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="b2a3b-110">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="b2a3b-110">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="b2a3b-111">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-111">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="b2a3b-112">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="b2a3b-112">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="b2a3b-113">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b2a3b-113">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="b2a3b-114">デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-114">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="b2a3b-115">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="b2a3b-115">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="b2a3b-116">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="b2a3b-116">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="b2a3b-117">デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-117">Get the number of unique users by device type over the selected time period.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
