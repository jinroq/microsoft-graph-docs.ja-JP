---
title: Yammer アクティビティ レポート
description: Yammer アクティビティ レポートを使用すると、組織全体での生成アクティビティの数と、Yammar でメッセージを投稿、「いいね!」を設定、メッセージを読み取ったそれぞれ別個のユーザーの数を確認することにより、Yammer への組織の関与のレベルを把握することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3ceda4e5771e442f4b664de71b595f8c5b6aeaf7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573607"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="b6997-103">Yammer アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="b6997-103">Yammer activity reports</span></span>

<span data-ttu-id="b6997-104">Yammer アクティビティ レポートを使用すると、組織全体での生成アクティビティの数と、Yammar でメッセージを投稿、「いいね!」を設定、メッセージを読み取ったそれぞれ別個のユーザーの数を確認することにより、Yammer への組織の関与のレベルを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="b6997-104">You can use the Yammer activity reports to understand the level of your organization's engagement with Yammer by seeing how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="b6997-105">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6997-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="b6997-106">レポート</span><span class="sxs-lookup"><span data-stu-id="b6997-106">Reports</span></span>

| <span data-ttu-id="b6997-107">関数</span><span class="sxs-lookup"><span data-stu-id="b6997-107">Function</span></span>                                 | <span data-ttu-id="b6997-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b6997-108">Return Type</span></span> | <span data-ttu-id="b6997-109">説明</span><span class="sxs-lookup"><span data-stu-id="b6997-109">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b6997-110">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="b6997-110">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="b6997-111">Stream</span><span class="sxs-lookup"><span data-stu-id="b6997-111">Stream</span></span>      | <span data-ttu-id="b6997-112">ユーザー別の Yammer アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="b6997-112">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="b6997-113">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="b6997-113">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="b6997-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b6997-114">Stream</span></span>      | <span data-ttu-id="b6997-115">投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="b6997-115">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="b6997-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="b6997-116">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="b6997-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b6997-117">Stream</span></span>      | <span data-ttu-id="b6997-118">Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="b6997-118">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
