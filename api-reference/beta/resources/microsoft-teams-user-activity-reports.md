---
title: Microsoft Teams ユーザー アクティビティ レポート
description: 組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 447aa9d36208ae9c966d86e733e99f81ab01e6ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517702"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="8f297-103">Microsoft Teams ユーザー アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="8f297-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f297-104">組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。</span><span class="sxs-lookup"><span data-stu-id="8f297-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="8f297-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f297-105">Methods</span></span>

| <span data-ttu-id="8f297-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f297-106">Method</span></span>                                   | <span data-ttu-id="8f297-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8f297-107">Return Type</span></span>                              | <span data-ttu-id="8f297-108">説明</span><span class="sxs-lookup"><span data-stu-id="8f297-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="8f297-109">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="8f297-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="8f297-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8f297-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="8f297-111">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f297-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="8f297-112">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8f297-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="8f297-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="8f297-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="8f297-114">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f297-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="8f297-115">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="8f297-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="8f297-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8f297-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="8f297-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8f297-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="8f297-118">アクティビティの種類ごとに、ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f297-118">Get the number of users by activity type.</span></span> <span data-ttu-id="8f297-119">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="8f297-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
