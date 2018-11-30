---
title: actionState 列挙型
description: デバイス上のアクションの状態
ms.openlocfilehash: e0169bd690cdc8a26cc771948ebcf311f6fd6aa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069722"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e0634-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e0634-103">actionState enum type</span></span>

> <span data-ttu-id="e0634-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0634-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0634-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0634-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0634-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0634-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0634-107">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="e0634-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="e0634-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0634-108">Members</span></span>
|<span data-ttu-id="e0634-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0634-109">Member</span></span>|<span data-ttu-id="e0634-110">値</span><span class="sxs-lookup"><span data-stu-id="e0634-110">Value</span></span>|<span data-ttu-id="e0634-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0634-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0634-112">none</span><span class="sxs-lookup"><span data-stu-id="e0634-112">none</span></span>|<span data-ttu-id="e0634-113">0</span><span class="sxs-lookup"><span data-stu-id="e0634-113">0</span></span>|<span data-ttu-id="e0634-114">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="e0634-114">Not a valid action state</span></span>|
|<span data-ttu-id="e0634-115">保留中</span><span class="sxs-lookup"><span data-stu-id="e0634-115">pending</span></span>|<span data-ttu-id="e0634-116">1</span><span class="sxs-lookup"><span data-stu-id="e0634-116">1</span></span>|<span data-ttu-id="e0634-117">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="e0634-117">Action is pending</span></span>|
|<span data-ttu-id="e0634-118">キャンセル</span><span class="sxs-lookup"><span data-stu-id="e0634-118">canceled</span></span>|<span data-ttu-id="e0634-119">2</span><span class="sxs-lookup"><span data-stu-id="e0634-119">2</span></span>|<span data-ttu-id="e0634-120">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="e0634-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="e0634-121">アクティブです</span><span class="sxs-lookup"><span data-stu-id="e0634-121">active</span></span>|<span data-ttu-id="e0634-122">3</span><span class="sxs-lookup"><span data-stu-id="e0634-122">3</span></span>|<span data-ttu-id="e0634-123">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="e0634-123">Action is active.</span></span>|
|<span data-ttu-id="e0634-124">done</span><span class="sxs-lookup"><span data-stu-id="e0634-124">done</span></span>|<span data-ttu-id="e0634-125">4</span><span class="sxs-lookup"><span data-stu-id="e0634-125">4</span></span>|<span data-ttu-id="e0634-126">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="e0634-126">Action completed without errors.</span></span>|
|<span data-ttu-id="e0634-127">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="e0634-127">failed</span></span>|<span data-ttu-id="e0634-128">5</span><span class="sxs-lookup"><span data-stu-id="e0634-128">5</span></span>|<span data-ttu-id="e0634-129">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="e0634-129">Action failed</span></span>|
|<span data-ttu-id="e0634-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="e0634-130">notSupported</span></span>|<span data-ttu-id="e0634-131">6</span><span class="sxs-lookup"><span data-stu-id="e0634-131">6</span></span>|<span data-ttu-id="e0634-132">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0634-132">Action is not supported.</span></span>|





