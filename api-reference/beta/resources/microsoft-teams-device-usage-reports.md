---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f9240f6cb310ada94f1a6694efb0da6cd691dc13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519907"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="38bfe-103">Microsoft Teams デバイスの使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="38bfe-103">Microsoft Teams device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38bfe-104">マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。</span><span class="sxs-lookup"><span data-stu-id="38bfe-104">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="38bfe-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="38bfe-105">Methods</span></span>

| <span data-ttu-id="38bfe-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="38bfe-106">Method</span></span>                                   | <span data-ttu-id="38bfe-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38bfe-107">Return Type</span></span>                              | <span data-ttu-id="38bfe-108">説明</span><span class="sxs-lookup"><span data-stu-id="38bfe-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="38bfe-109">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="38bfe-109">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="38bfe-110">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="38bfe-110">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="38bfe-111">ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="38bfe-111">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="38bfe-112">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="38bfe-112">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="38bfe-113">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="38bfe-113">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="38bfe-114">デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="38bfe-114">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="38bfe-115">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="38bfe-115">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="38bfe-116">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="38bfe-116">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="38bfe-117">デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="38bfe-117">Get the number of unique users by device type over the selected time period.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
