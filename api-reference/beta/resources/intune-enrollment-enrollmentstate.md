---
title: enrollmentState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a3790733067598442af615cb90b8ae347fd228
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869021"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="3b7d5-103">enrollmentState 列挙型</span><span class="sxs-lookup"><span data-stu-id="3b7d5-103">enrollmentState enum type</span></span>

> <span data-ttu-id="3b7d5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b7d5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b7d5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b7d5-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3b7d5-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="3b7d5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b7d5-108">Members</span></span>
|<span data-ttu-id="3b7d5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b7d5-109">Member</span></span>|<span data-ttu-id="3b7d5-110">値</span><span class="sxs-lookup"><span data-stu-id="3b7d5-110">Value</span></span>|<span data-ttu-id="3b7d5-111">説明</span><span class="sxs-lookup"><span data-stu-id="3b7d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b7d5-112">不明</span><span class="sxs-lookup"><span data-stu-id="3b7d5-112">unknown</span></span>|<span data-ttu-id="3b7d5-113">0</span><span class="sxs-lookup"><span data-stu-id="3b7d5-113">0</span></span>|<span data-ttu-id="3b7d5-114">デバイス登録の状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="3b7d5-115">登録</span><span class="sxs-lookup"><span data-stu-id="3b7d5-115">enrolled</span></span>|<span data-ttu-id="3b7d5-116">1</span><span class="sxs-lookup"><span data-stu-id="3b7d5-116">1</span></span>|<span data-ttu-id="3b7d5-117">デバイスを登録します。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="3b7d5-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="3b7d5-118">pendingReset</span></span>|<span data-ttu-id="3b7d5-119">2</span><span class="sxs-lookup"><span data-stu-id="3b7d5-119">2</span></span>|<span data-ttu-id="3b7d5-120">登録され、登録プロファイルを使用して登録されているが、登録されているプロファイルが割り当てられているプロファイルとは異なる。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="3b7d5-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-121">failed</span></span>|<span data-ttu-id="3b7d5-122">3</span><span class="sxs-lookup"><span data-stu-id="3b7d5-122">3</span></span>|<span data-ttu-id="3b7d5-123">登録していない登録に失敗したレコードがあるとします。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="3b7d5-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="3b7d5-124">notContacted</span></span>|<span data-ttu-id="3b7d5-125">4</span><span class="sxs-lookup"><span data-stu-id="3b7d5-125">4</span></span>|<span data-ttu-id="3b7d5-126">デバイスをインポートしていますが、登録していません。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="3b7d5-127">ブロック</span><span class="sxs-lookup"><span data-stu-id="3b7d5-127">blocked</span></span>|<span data-ttu-id="3b7d5-128">5</span><span class="sxs-lookup"><span data-stu-id="3b7d5-128">5</span></span>|<span data-ttu-id="3b7d5-129">デバイスが、userless として登録されて、アプリケーションのインストールに失敗したため、ユーザー登録への移動がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="3b7d5-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





