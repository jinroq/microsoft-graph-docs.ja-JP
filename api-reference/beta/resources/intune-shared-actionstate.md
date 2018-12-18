---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
ms.openlocfilehash: 1f36c3a6709ade5860ff24cc8d10c2cb0294a471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315107"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="9c426-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="9c426-103">actionState enum type</span></span>

> <span data-ttu-id="9c426-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c426-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c426-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c426-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c426-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c426-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c426-107">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="9c426-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="9c426-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c426-108">Members</span></span>
|<span data-ttu-id="9c426-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c426-109">Member</span></span>|<span data-ttu-id="9c426-110">値</span><span class="sxs-lookup"><span data-stu-id="9c426-110">Value</span></span>|<span data-ttu-id="9c426-111">説明</span><span class="sxs-lookup"><span data-stu-id="9c426-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c426-112">none</span><span class="sxs-lookup"><span data-stu-id="9c426-112">none</span></span>|<span data-ttu-id="9c426-113">0</span><span class="sxs-lookup"><span data-stu-id="9c426-113">0</span></span>|<span data-ttu-id="9c426-114">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="9c426-114">Not a valid action state</span></span>|
|<span data-ttu-id="9c426-115">保留中</span><span class="sxs-lookup"><span data-stu-id="9c426-115">pending</span></span>|<span data-ttu-id="9c426-116">1</span><span class="sxs-lookup"><span data-stu-id="9c426-116">1</span></span>|<span data-ttu-id="9c426-117">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="9c426-117">Action is pending</span></span>|
|<span data-ttu-id="9c426-118">キャンセル</span><span class="sxs-lookup"><span data-stu-id="9c426-118">canceled</span></span>|<span data-ttu-id="9c426-119">2</span><span class="sxs-lookup"><span data-stu-id="9c426-119">2</span></span>|<span data-ttu-id="9c426-120">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="9c426-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="9c426-121">アクティブです</span><span class="sxs-lookup"><span data-stu-id="9c426-121">active</span></span>|<span data-ttu-id="9c426-122">3</span><span class="sxs-lookup"><span data-stu-id="9c426-122">3</span></span>|<span data-ttu-id="9c426-123">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="9c426-123">Action is active.</span></span>|
|<span data-ttu-id="9c426-124">done</span><span class="sxs-lookup"><span data-stu-id="9c426-124">done</span></span>|<span data-ttu-id="9c426-125">4</span><span class="sxs-lookup"><span data-stu-id="9c426-125">4</span></span>|<span data-ttu-id="9c426-126">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="9c426-126">Action completed without errors.</span></span>|
|<span data-ttu-id="9c426-127">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9c426-127">failed</span></span>|<span data-ttu-id="9c426-128">5</span><span class="sxs-lookup"><span data-stu-id="9c426-128">5</span></span>|<span data-ttu-id="9c426-129">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="9c426-129">Action failed</span></span>|
|<span data-ttu-id="9c426-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="9c426-130">notSupported</span></span>|<span data-ttu-id="9c426-131">6</span><span class="sxs-lookup"><span data-stu-id="9c426-131">6</span></span>|<span data-ttu-id="9c426-132">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c426-132">Action is not supported.</span></span>|





