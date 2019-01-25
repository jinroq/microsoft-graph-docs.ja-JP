---
title: Skype for Business ピア ツー ピア アクティビティ レポート
description: 組織全体でピア ツー ピア アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a85913f1f8d97d932f5ed97d0eb02d821acf111d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513957"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="8400c-104">Skype for Business ピア ツー ピア アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="8400c-104">Skype for Business peer-to-peer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8400c-105">組織全体でピア ツー ピア アクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8400c-105">You can get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="8400c-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="8400c-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="8400c-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8400c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="8400c-108">レポート</span><span class="sxs-lookup"><span data-stu-id="8400c-108">Reports</span></span>

| <span data-ttu-id="8400c-109">関数</span><span class="sxs-lookup"><span data-stu-id="8400c-109">Function</span></span>                                 | <span data-ttu-id="8400c-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8400c-110">CSV return type</span></span> | <span data-ttu-id="8400c-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8400c-111">JSON return type</span></span>                         | <span data-ttu-id="8400c-112">説明</span><span class="sxs-lookup"><span data-stu-id="8400c-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="8400c-113">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8400c-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="8400c-114">Stream</span><span class="sxs-lookup"><span data-stu-id="8400c-114">Stream</span></span>          | [<span data-ttu-id="8400c-115">skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="8400c-115">skypeForBusinessPeerToPeerActivityCounts</span></span>](../resources/skypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="8400c-116">組織内で実施されたセッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="8400c-116">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="8400c-117">セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="8400c-117">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="8400c-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8400c-118">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="8400c-119">ストリーム</span><span class="sxs-lookup"><span data-stu-id="8400c-119">Stream</span></span>          | [<span data-ttu-id="8400c-120">skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8400c-120">skypeForBusinessPeerToPeerActivityUserCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="8400c-121">組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="8400c-121">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="8400c-122">ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="8400c-122">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="8400c-123">時間 (分) を取得する</span><span class="sxs-lookup"><span data-stu-id="8400c-123">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="8400c-124">Stream</span><span class="sxs-lookup"><span data-stu-id="8400c-124">Stream</span></span>          | [<span data-ttu-id="8400c-125">skypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="8400c-125">skypeForBusinessPeerToPeerActivityMinuteCounts</span></span>](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="8400c-126">組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="8400c-126">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="8400c-127">セッションの種類には、オーディオとビデオが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8400c-127">Types of sessions include audio and video.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-peer-to-peer-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
