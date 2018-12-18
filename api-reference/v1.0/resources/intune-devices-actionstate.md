---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
ms.openlocfilehash: 53ee72430ac646bf978a3167b87feaf398c8ac37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333384"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e0a6a-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e0a6a-103">actionState enum type</span></span>

> <span data-ttu-id="e0a6a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0a6a-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="e0a6a-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="e0a6a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0a6a-106">Members</span></span>
|<span data-ttu-id="e0a6a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0a6a-107">Member</span></span>|<span data-ttu-id="e0a6a-108">値</span><span class="sxs-lookup"><span data-stu-id="e0a6a-108">Value</span></span>|<span data-ttu-id="e0a6a-109">説明</span><span class="sxs-lookup"><span data-stu-id="e0a6a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0a6a-110">none</span><span class="sxs-lookup"><span data-stu-id="e0a6a-110">none</span></span>|<span data-ttu-id="e0a6a-111">0</span><span class="sxs-lookup"><span data-stu-id="e0a6a-111">0</span></span>|<span data-ttu-id="e0a6a-112">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="e0a6a-112">Not a valid action state</span></span>|
|<span data-ttu-id="e0a6a-113">保留中</span><span class="sxs-lookup"><span data-stu-id="e0a6a-113">pending</span></span>|<span data-ttu-id="e0a6a-114">1</span><span class="sxs-lookup"><span data-stu-id="e0a6a-114">1</span></span>|<span data-ttu-id="e0a6a-115">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-115">Action is pending</span></span>|
|<span data-ttu-id="e0a6a-116">キャンセル</span><span class="sxs-lookup"><span data-stu-id="e0a6a-116">canceled</span></span>|<span data-ttu-id="e0a6a-117">2</span><span class="sxs-lookup"><span data-stu-id="e0a6a-117">2</span></span>|<span data-ttu-id="e0a6a-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="e0a6a-119">アクティブです</span><span class="sxs-lookup"><span data-stu-id="e0a6a-119">active</span></span>|<span data-ttu-id="e0a6a-120">3</span><span class="sxs-lookup"><span data-stu-id="e0a6a-120">3</span></span>|<span data-ttu-id="e0a6a-121">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-121">Action is active.</span></span>|
|<span data-ttu-id="e0a6a-122">done</span><span class="sxs-lookup"><span data-stu-id="e0a6a-122">done</span></span>|<span data-ttu-id="e0a6a-123">4</span><span class="sxs-lookup"><span data-stu-id="e0a6a-123">4</span></span>|<span data-ttu-id="e0a6a-124">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-124">Action completed without errors.</span></span>|
|<span data-ttu-id="e0a6a-125">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-125">failed</span></span>|<span data-ttu-id="e0a6a-126">5</span><span class="sxs-lookup"><span data-stu-id="e0a6a-126">5</span></span>|<span data-ttu-id="e0a6a-127">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="e0a6a-127">Action failed</span></span>|
|<span data-ttu-id="e0a6a-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="e0a6a-128">notSupported</span></span>|<span data-ttu-id="e0a6a-129">6</span><span class="sxs-lookup"><span data-stu-id="e0a6a-129">6</span></span>|<span data-ttu-id="e0a6a-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0a6a-130">Action is not supported.</span></span>|



