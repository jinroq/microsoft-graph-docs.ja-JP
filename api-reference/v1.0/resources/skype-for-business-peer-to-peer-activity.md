---
title: Skype for Business ピア ツー ピア アクティビティ レポート
description: Skype for Business ピア ツー ピア アクティビティ レポートを使用して、組織全体のピア ツー ピア アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 6c94b4fd09fb71af3c264664eaa0182256dfa949
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920731"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="a8e4d-104">Skype for Business ピア ツー ピア アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="a8e4d-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="a8e4d-105">Skype for Business ピア ツー ピア アクティビティ レポートを使用して、組織全体のピア ツー ピア アクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-105">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="a8e4d-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="a8e4d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="a8e4d-108">レポート</span><span class="sxs-lookup"><span data-stu-id="a8e4d-108">Reports</span></span>

| <span data-ttu-id="a8e4d-109">関数</span><span class="sxs-lookup"><span data-stu-id="a8e4d-109">Function</span></span>                                 | <span data-ttu-id="a8e4d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a8e4d-110">Return Type</span></span> | <span data-ttu-id="a8e4d-111">説明</span><span class="sxs-lookup"><span data-stu-id="a8e4d-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="a8e4d-112">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="a8e4d-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="a8e4d-113">Stream</span><span class="sxs-lookup"><span data-stu-id="a8e4d-113">Stream</span></span>      | <span data-ttu-id="a8e4d-114">組織内で実施されたセッションの数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-114">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="a8e4d-115">セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-115">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="a8e4d-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="a8e4d-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="a8e4d-117">Stream</span><span class="sxs-lookup"><span data-stu-id="a8e4d-117">Stream</span></span>      | <span data-ttu-id="a8e4d-118">組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-118">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="a8e4d-119">ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-119">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="a8e4d-120">時間 (分) を取得する</span><span class="sxs-lookup"><span data-stu-id="a8e4d-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="a8e4d-121">Stream</span><span class="sxs-lookup"><span data-stu-id="a8e4d-121">Stream</span></span>      | <span data-ttu-id="a8e4d-122">組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-122">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="a8e4d-123">セッションの種類には、オーディオとビデオが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a8e4d-123">Types of sessions include audio and video.</span></span> |

