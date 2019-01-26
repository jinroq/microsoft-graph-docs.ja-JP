---
title: Skype for Business 参加者アクティビティ レポート
description: 組織全体にわたって会議活動の詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 31810a7ca5df52724089783efe208e5a28bf0cfb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576746"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="be906-104">Skype for Business 参加者アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="be906-104">Skype for Business participant activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be906-105">組織全体にわたって会議活動の詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="be906-105">You can get details on conferencing activity across your organization.</span></span> <span data-ttu-id="be906-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="be906-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="be906-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be906-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="be906-108">レポート</span><span class="sxs-lookup"><span data-stu-id="be906-108">Reports</span></span>

| <span data-ttu-id="be906-109">関数</span><span class="sxs-lookup"><span data-stu-id="be906-109">Function</span></span>                                 | <span data-ttu-id="be906-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be906-110">CSV return type</span></span> | <span data-ttu-id="be906-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be906-111">JSON return type</span></span>                         | <span data-ttu-id="be906-112">説明</span><span class="sxs-lookup"><span data-stu-id="be906-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="be906-113">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="be906-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="be906-114">Stream</span><span class="sxs-lookup"><span data-stu-id="be906-114">Stream</span></span>          | [<span data-ttu-id="be906-115">skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="be906-115">skypeForBusinessParticipantActivityCounts</span></span>](../resources/skypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="be906-116">組織からユーザーが参加した会議セッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="be906-116">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="be906-117">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="be906-117">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="be906-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="be906-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="be906-119">Stream</span><span class="sxs-lookup"><span data-stu-id="be906-119">Stream</span></span>          | [<span data-ttu-id="be906-120">skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="be906-120">skypeForBusinessParticipantActivityUserCounts</span></span>](../resources/skypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="be906-121">組織からユーザーが参加したそれぞれ別個のユーザーの数と会議セッションの種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="be906-121">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="be906-122">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="be906-122">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="be906-123">時間 (分) を取得する</span><span class="sxs-lookup"><span data-stu-id="be906-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="be906-124">Stream</span><span class="sxs-lookup"><span data-stu-id="be906-124">Stream</span></span>          | [<span data-ttu-id="be906-125">skypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="be906-125">skypeForBusinessParticipantActivityMinuteCounts</span></span>](../resources/skypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="be906-126">組織からユーザーが参加した会議セッションの長さ (分) と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="be906-126">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="be906-127">会議セッションの種類には、オーディオ/ビデオがあります。</span><span class="sxs-lookup"><span data-stu-id="be906-127">Types of conference sessions include audio/video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-participant-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
