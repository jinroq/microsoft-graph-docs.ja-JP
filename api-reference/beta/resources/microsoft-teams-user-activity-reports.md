---
title: Microsoft Teams ユーザー アクティビティ レポート
description: microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457082"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="8391b-103">Microsoft Teams ユーザー アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="8391b-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8391b-104">microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="8391b-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="8391b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8391b-105">Methods</span></span>

| <span data-ttu-id="8391b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8391b-106">Method</span></span>                                   | <span data-ttu-id="8391b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8391b-107">Return Type</span></span>                              | <span data-ttu-id="8391b-108">説明</span><span class="sxs-lookup"><span data-stu-id="8391b-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="8391b-109">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="8391b-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="8391b-110">teamsuseractivityuserdetail</span><span class="sxs-lookup"><span data-stu-id="8391b-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="8391b-111">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8391b-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="8391b-112">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8391b-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="8391b-113">teamsuseractivitycounts</span><span class="sxs-lookup"><span data-stu-id="8391b-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="8391b-114">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8391b-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="8391b-115">アクティビティの種類は、チームのチャット メッセージ数、プライベート チャット メッセージ数、コール数、または会議数です。</span><span class="sxs-lookup"><span data-stu-id="8391b-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="8391b-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8391b-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="8391b-117">teamsuseractivityusercounts</span><span class="sxs-lookup"><span data-stu-id="8391b-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="8391b-118">アクティビティの種類ごとに、ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="8391b-118">Get the number of users by activity type.</span></span> <span data-ttu-id="8391b-119">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="8391b-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
