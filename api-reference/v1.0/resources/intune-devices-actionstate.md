---
title: actionState 列挙型
description: デバイス上のアクションの状態
ms.openlocfilehash: 1a18eb87cb4c9162777d16dc866de5f5766c87b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023732"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e461a-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e461a-103">actionState enum type</span></span>

> <span data-ttu-id="e461a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e461a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e461a-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="e461a-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="e461a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e461a-106">Members</span></span>
|<span data-ttu-id="e461a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e461a-107">Member</span></span>|<span data-ttu-id="e461a-108">値</span><span class="sxs-lookup"><span data-stu-id="e461a-108">Value</span></span>|<span data-ttu-id="e461a-109">説明</span><span class="sxs-lookup"><span data-stu-id="e461a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e461a-110">none</span><span class="sxs-lookup"><span data-stu-id="e461a-110">none</span></span>|<span data-ttu-id="e461a-111">0</span><span class="sxs-lookup"><span data-stu-id="e461a-111">0</span></span>|<span data-ttu-id="e461a-112">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="e461a-112">Not a valid action state</span></span>|
|<span data-ttu-id="e461a-113">保留中</span><span class="sxs-lookup"><span data-stu-id="e461a-113">pending</span></span>|<span data-ttu-id="e461a-114">1</span><span class="sxs-lookup"><span data-stu-id="e461a-114">1</span></span>|<span data-ttu-id="e461a-115">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="e461a-115">Action is pending</span></span>|
|<span data-ttu-id="e461a-116">キャンセル</span><span class="sxs-lookup"><span data-stu-id="e461a-116">canceled</span></span>|<span data-ttu-id="e461a-117">2</span><span class="sxs-lookup"><span data-stu-id="e461a-117">2</span></span>|<span data-ttu-id="e461a-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="e461a-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="e461a-119">アクティブです</span><span class="sxs-lookup"><span data-stu-id="e461a-119">active</span></span>|<span data-ttu-id="e461a-120">3</span><span class="sxs-lookup"><span data-stu-id="e461a-120">3</span></span>|<span data-ttu-id="e461a-121">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="e461a-121">Action is active.</span></span>|
|<span data-ttu-id="e461a-122">done</span><span class="sxs-lookup"><span data-stu-id="e461a-122">done</span></span>|<span data-ttu-id="e461a-123">4</span><span class="sxs-lookup"><span data-stu-id="e461a-123">4</span></span>|<span data-ttu-id="e461a-124">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="e461a-124">Action completed without errors.</span></span>|
|<span data-ttu-id="e461a-125">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="e461a-125">failed</span></span>|<span data-ttu-id="e461a-126">5</span><span class="sxs-lookup"><span data-stu-id="e461a-126">5</span></span>|<span data-ttu-id="e461a-127">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="e461a-127">Action failed</span></span>|
|<span data-ttu-id="e461a-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="e461a-128">notSupported</span></span>|<span data-ttu-id="e461a-129">6</span><span class="sxs-lookup"><span data-stu-id="e461a-129">6</span></span>|<span data-ttu-id="e461a-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e461a-130">Action is not supported.</span></span>|



