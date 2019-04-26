---
title: Microsoft Teams ユーザー アクティビティ レポート
description: microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f88d1c9d568ce3fbbf9bfe19abaf637065d37b8c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342206"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="7bb6b-103">Microsoft Teams ユーザー アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="7bb6b-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bb6b-104">microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="7bb6b-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="7bb6b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7bb6b-105">Methods</span></span>

| <span data-ttu-id="7bb6b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7bb6b-106">Method</span></span>                                   | <span data-ttu-id="7bb6b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7bb6b-107">Return Type</span></span>                              | <span data-ttu-id="7bb6b-108">説明</span><span class="sxs-lookup"><span data-stu-id="7bb6b-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="7bb6b-109">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="7bb6b-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="7bb6b-110">teamsuseractivityuserdetail</span><span class="sxs-lookup"><span data-stu-id="7bb6b-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="7bb6b-111">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="7bb6b-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="7bb6b-112">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="7bb6b-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="7bb6b-113">teamsuseractivitycounts</span><span class="sxs-lookup"><span data-stu-id="7bb6b-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="7bb6b-114">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7bb6b-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="7bb6b-115">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="7bb6b-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="7bb6b-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="7bb6b-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="7bb6b-117">teamsuseractivityusercounts</span><span class="sxs-lookup"><span data-stu-id="7bb6b-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="7bb6b-118">アクティビティの種類ごとに、ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7bb6b-118">Get the number of users by activity type.</span></span> <span data-ttu-id="7bb6b-119">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="7bb6b-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
