---
title: Microsoft Teams ユーザー アクティビティ レポート
description: 組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2dd3ed3cde8f1a00ae7a48336bfaef857721f046
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991434"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="cbc66-103">Microsoft Teams ユーザー アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="cbc66-103">Microsoft Teams user activity reports</span></span>

> <span data-ttu-id="cbc66-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cbc66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbc66-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbc66-105">Use of these APIs in production applications is not supported.</span></span> <span data-ttu-id="cbc66-106">21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbc66-106">These APIs are not supported in Microsoft Graph China operated by 21Vianet.</span></span>

<span data-ttu-id="cbc66-107">組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。</span><span class="sxs-lookup"><span data-stu-id="cbc66-107">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="cbc66-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbc66-108">Methods</span></span>

| <span data-ttu-id="cbc66-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbc66-109">Method</span></span>                                   | <span data-ttu-id="cbc66-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbc66-110">Return Type</span></span>                              | <span data-ttu-id="cbc66-111">説明</span><span class="sxs-lookup"><span data-stu-id="cbc66-111">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="cbc66-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="cbc66-112">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="cbc66-113">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="cbc66-113">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="cbc66-114">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="cbc66-114">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="cbc66-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="cbc66-115">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="cbc66-116">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="cbc66-116">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="cbc66-117">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="cbc66-117">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="cbc66-118">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="cbc66-118">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="cbc66-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="cbc66-119">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="cbc66-120">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cbc66-120">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="cbc66-121">アクティビティの種類ごとに、ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="cbc66-121">Get the number of users by activity type.</span></span> <span data-ttu-id="cbc66-122">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="cbc66-122">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
