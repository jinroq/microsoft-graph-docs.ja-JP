---
title: Microsoft Teams ユーザー アクティビティ レポート
description: 組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。
localization_priority: Normal
ms.openlocfilehash: 2fc2eee8243a338204687114d2f1de3d2e794a9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845522"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="fef42-103">Microsoft Teams ユーザー アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="fef42-103">Microsoft Teams user activity reports</span></span>

> <span data-ttu-id="fef42-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fef42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fef42-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef42-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="fef42-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef42-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="fef42-107">組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。</span><span class="sxs-lookup"><span data-stu-id="fef42-107">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="fef42-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fef42-108">Methods</span></span>

| <span data-ttu-id="fef42-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fef42-109">Method</span></span>                                   | <span data-ttu-id="fef42-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fef42-110">Return Type</span></span>                              | <span data-ttu-id="fef42-111">説明</span><span class="sxs-lookup"><span data-stu-id="fef42-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="fef42-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="fef42-112">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="fef42-113">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fef42-113">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="fef42-114">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="fef42-114">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="fef42-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fef42-115">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="fef42-116">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="fef42-116">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="fef42-117">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fef42-117">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="fef42-118">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="fef42-118">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="fef42-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fef42-119">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="fef42-120">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fef42-120">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="fef42-121">アクティビティの種類ごとに、ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fef42-121">Get the number of users by activity type.</span></span> <span data-ttu-id="fef42-122">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="fef42-122">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
