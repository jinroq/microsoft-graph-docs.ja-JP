---
title: Microsoft Teams ユーザー アクティビティ レポート
description: Microsoft Teams ユーザーアクティビティレポートを使用して、組織内の Microsoft Teams ユーザーアクティビティの洞察を得ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ca8d1f772744b33aa5fee60fc3b843bf60b0be9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009637"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="f32f9-103">Microsoft Teams ユーザー アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="f32f9-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f32f9-104">Microsoft Teams ユーザーアクティビティレポートを使用して、組織内の Microsoft Teams ユーザーアクティビティの洞察を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="f32f9-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f32f9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f32f9-105">Methods</span></span>

| <span data-ttu-id="f32f9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f32f9-106">Method</span></span>                                   | <span data-ttu-id="f32f9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f32f9-107">Return Type</span></span>                              | <span data-ttu-id="f32f9-108">説明</span><span class="sxs-lookup"><span data-stu-id="f32f9-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="f32f9-109">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="f32f9-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="f32f9-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f32f9-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="f32f9-111">ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="f32f9-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="f32f9-112">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="f32f9-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="f32f9-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f32f9-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="f32f9-114">アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="f32f9-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="f32f9-115">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="f32f9-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="f32f9-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="f32f9-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="f32f9-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f32f9-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="f32f9-118">アクティビティの種類ごとに、ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="f32f9-118">Get the number of users by activity type.</span></span> <span data-ttu-id="f32f9-119">アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。</span><span class="sxs-lookup"><span data-stu-id="f32f9-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
