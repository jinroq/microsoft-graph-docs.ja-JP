---
title: Skype for Business 参加者アクティビティ レポート
description: 組織全体の会議アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 31810a7ca5df52724089783efe208e5a28bf0cfb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554864"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="ce25d-104">Skype for Business 参加者アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="ce25d-104">Skype for Business participant activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce25d-105">組織全体の会議アクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="ce25d-105">You can get details on conferencing activity across your organization.</span></span> <span data-ttu-id="ce25d-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="ce25d-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="ce25d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce25d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="ce25d-108">レポート</span><span class="sxs-lookup"><span data-stu-id="ce25d-108">Reports</span></span>

| <span data-ttu-id="ce25d-109">関数</span><span class="sxs-lookup"><span data-stu-id="ce25d-109">Function</span></span>                                 | <span data-ttu-id="ce25d-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce25d-110">CSV return type</span></span> | <span data-ttu-id="ce25d-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="ce25d-111">JSON return type</span></span>                         | <span data-ttu-id="ce25d-112">説明</span><span class="sxs-lookup"><span data-stu-id="ce25d-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ce25d-113">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ce25d-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="ce25d-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="ce25d-114">Stream</span></span>          | [<span data-ttu-id="ce25d-115">skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ce25d-115">skypeForBusinessParticipantActivityCounts</span></span>](../resources/skypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="ce25d-116">組織からユーザーが参加した会議セッションの数と種類ついて、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce25d-116">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="ce25d-117">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="ce25d-117">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="ce25d-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ce25d-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="ce25d-119">Stream</span><span class="sxs-lookup"><span data-stu-id="ce25d-119">Stream</span></span>          | [<span data-ttu-id="ce25d-120">skypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ce25d-120">skypeForBusinessParticipantActivityUserCounts</span></span>](../resources/skypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="ce25d-121">組織からユーザーが参加したそれぞれ別個のユーザーの数と会議セッションの種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce25d-121">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="ce25d-122">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="ce25d-122">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="ce25d-123">時間 (分) を取得する</span><span class="sxs-lookup"><span data-stu-id="ce25d-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="ce25d-124">Stream</span><span class="sxs-lookup"><span data-stu-id="ce25d-124">Stream</span></span>          | [<span data-ttu-id="ce25d-125">skypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="ce25d-125">skypeForBusinessParticipantActivityMinuteCounts</span></span>](../resources/skypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="ce25d-126">組織からユーザーが参加した会議セッションの長さ (分) と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce25d-126">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="ce25d-127">会議セッションの種類には、オーディオ/ビデオがあります。</span><span class="sxs-lookup"><span data-stu-id="ce25d-127">Types of conference sessions include audio/video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-participant-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
