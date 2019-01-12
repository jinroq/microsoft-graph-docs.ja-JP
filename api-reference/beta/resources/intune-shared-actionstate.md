---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ec93848deccb7d6bb21331095f9ecf4a881815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990853"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e44d1-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e44d1-103">actionState enum type</span></span>

> <span data-ttu-id="e44d1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e44d1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e44d1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e44d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e44d1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e44d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e44d1-107">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="e44d1-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="e44d1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e44d1-108">Members</span></span>
|<span data-ttu-id="e44d1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e44d1-109">Member</span></span>|<span data-ttu-id="e44d1-110">値</span><span class="sxs-lookup"><span data-stu-id="e44d1-110">Value</span></span>|<span data-ttu-id="e44d1-111">説明</span><span class="sxs-lookup"><span data-stu-id="e44d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44d1-112">none</span><span class="sxs-lookup"><span data-stu-id="e44d1-112">none</span></span>|<span data-ttu-id="e44d1-113">0</span><span class="sxs-lookup"><span data-stu-id="e44d1-113">0</span></span>|<span data-ttu-id="e44d1-114">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="e44d1-114">Not a valid action state</span></span>|
|<span data-ttu-id="e44d1-115">保留中</span><span class="sxs-lookup"><span data-stu-id="e44d1-115">pending</span></span>|<span data-ttu-id="e44d1-116">1</span><span class="sxs-lookup"><span data-stu-id="e44d1-116">1</span></span>|<span data-ttu-id="e44d1-117">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="e44d1-117">Action is pending</span></span>|
|<span data-ttu-id="e44d1-118">キャンセル</span><span class="sxs-lookup"><span data-stu-id="e44d1-118">canceled</span></span>|<span data-ttu-id="e44d1-119">2</span><span class="sxs-lookup"><span data-stu-id="e44d1-119">2</span></span>|<span data-ttu-id="e44d1-120">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="e44d1-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="e44d1-121">アクティブです</span><span class="sxs-lookup"><span data-stu-id="e44d1-121">active</span></span>|<span data-ttu-id="e44d1-122">3</span><span class="sxs-lookup"><span data-stu-id="e44d1-122">3</span></span>|<span data-ttu-id="e44d1-123">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="e44d1-123">Action is active.</span></span>|
|<span data-ttu-id="e44d1-124">done</span><span class="sxs-lookup"><span data-stu-id="e44d1-124">done</span></span>|<span data-ttu-id="e44d1-125">4</span><span class="sxs-lookup"><span data-stu-id="e44d1-125">4</span></span>|<span data-ttu-id="e44d1-126">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="e44d1-126">Action completed without errors.</span></span>|
|<span data-ttu-id="e44d1-127">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="e44d1-127">failed</span></span>|<span data-ttu-id="e44d1-128">5</span><span class="sxs-lookup"><span data-stu-id="e44d1-128">5</span></span>|<span data-ttu-id="e44d1-129">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="e44d1-129">Action failed</span></span>|
|<span data-ttu-id="e44d1-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="e44d1-130">notSupported</span></span>|<span data-ttu-id="e44d1-131">6</span><span class="sxs-lookup"><span data-stu-id="e44d1-131">6</span></span>|<span data-ttu-id="e44d1-132">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e44d1-132">Action is not supported.</span></span>|





