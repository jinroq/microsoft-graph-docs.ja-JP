---
title: Skype for Business アクティビティ レポート
description: Skype for Business アクティビティ レポートを使用して、組織全体のアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a98e74c1c94f1b94046aea0a5b2964d47f55595b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552782"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="6368b-104">Skype for Business アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="6368b-104">Skype for Business activity reports</span></span>

<span data-ttu-id="6368b-105">Skype for Business アクティビティ レポートを使用して、組織全体のアクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="6368b-105">You can use the Skype for Business activity reports to get details on activity across your organization.</span></span> <span data-ttu-id="6368b-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="6368b-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="6368b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6368b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="6368b-108">レポート</span><span class="sxs-lookup"><span data-stu-id="6368b-108">Reports</span></span>

| <span data-ttu-id="6368b-109">関数</span><span class="sxs-lookup"><span data-stu-id="6368b-109">Function</span></span>                                 | <span data-ttu-id="6368b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6368b-110">Return Type</span></span> | <span data-ttu-id="6368b-111">説明</span><span class="sxs-lookup"><span data-stu-id="6368b-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="6368b-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="6368b-112">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="6368b-113">Stream</span><span class="sxs-lookup"><span data-stu-id="6368b-113">Stream</span></span>      | <span data-ttu-id="6368b-114">ユーザー別の Skype for Business アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="6368b-114">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="6368b-115">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="6368b-115">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="6368b-116">Stream</span><span class="sxs-lookup"><span data-stu-id="6368b-116">Stream</span></span>      | <span data-ttu-id="6368b-117">Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="6368b-117">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="6368b-118">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="6368b-118">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="6368b-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="6368b-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="6368b-120">Stream</span><span class="sxs-lookup"><span data-stu-id="6368b-120">Stream</span></span>      | <span data-ttu-id="6368b-121">Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="6368b-121">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="6368b-122">レポートには、ピア ツー ピア セッションの数も含まれます。</span><span class="sxs-lookup"><span data-stu-id="6368b-122">The report also includes the number of peer-to-peer sessions.</span></span> |
