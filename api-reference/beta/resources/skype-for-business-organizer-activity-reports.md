---
title: Skype for Business 開催者アクティビティ レポート
description: 組織全体で開催された会議アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8254221fc32b299b4d1a1de48165f6349b739f22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568188"
---
# <a name="skype-for-business-organizer-activity-reports"></a><span data-ttu-id="7b9dd-104">Skype for Business 開催者アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="7b9dd-104">Skype for Business organizer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b9dd-105">組織全体で開催された会議アクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-105">You can get details on organized conferences activity across your organization.</span></span> <span data-ttu-id="7b9dd-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="7b9dd-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="reports"></a><span data-ttu-id="7b9dd-108">レポート</span><span class="sxs-lookup"><span data-stu-id="7b9dd-108">Reports</span></span>

| <span data-ttu-id="7b9dd-109">関数</span><span class="sxs-lookup"><span data-stu-id="7b9dd-109">Function</span></span>                                 | <span data-ttu-id="7b9dd-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7b9dd-110">CSV return type</span></span> | <span data-ttu-id="7b9dd-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="7b9dd-111">JSON return type</span></span>                         | <span data-ttu-id="7b9dd-112">説明</span><span class="sxs-lookup"><span data-stu-id="7b9dd-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7b9dd-113">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="7b9dd-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="7b9dd-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="7b9dd-114">Stream</span></span>          | [<span data-ttu-id="7b9dd-115">skypeforbusinessオーガナイザー eractivity計数</span><span class="sxs-lookup"><span data-stu-id="7b9dd-115">skypeForBusinessOrganizerActivityCounts</span></span>](../resources/skypeforbusinessorganizeractivitycounts.md) | <span data-ttu-id="7b9dd-116">組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-116">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7b9dd-117">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-117">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="7b9dd-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="7b9dd-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="7b9dd-119">Stream</span><span class="sxs-lookup"><span data-stu-id="7b9dd-119">Stream</span></span>          | [<span data-ttu-id="7b9dd-120">skypeforbusinessオーガナイザー eractivityuser計数</span><span class="sxs-lookup"><span data-stu-id="7b9dd-120">skypeForBusinessOrganizerActivityUserCounts</span></span>](../resources/skypeforbusinessorganizeractivityusercounts.md) | <span data-ttu-id="7b9dd-121">一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-121">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7b9dd-122">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-122">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span> |
| [<span data-ttu-id="7b9dd-123">時間 (分) を取得する</span><span class="sxs-lookup"><span data-stu-id="7b9dd-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="7b9dd-124">Stream</span><span class="sxs-lookup"><span data-stu-id="7b9dd-124">Stream</span></span>          | [<span data-ttu-id="7b9dd-125">skypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="7b9dd-125">skypeForBusinessOrganizerActivityMinuteCounts</span></span>](../resources/skypeforbusinessorganizeractivityminutecounts.md) | <span data-ttu-id="7b9dd-126">組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-126">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7b9dd-127">電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。</span><span class="sxs-lookup"><span data-stu-id="7b9dd-127">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-organizer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
