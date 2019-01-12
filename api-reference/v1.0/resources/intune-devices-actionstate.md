---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5579d8de986a764cd96e42dff30c007449130b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922446"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="f1611-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f1611-103">actionState enum type</span></span>

> <span data-ttu-id="f1611-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1611-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1611-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="f1611-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="f1611-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f1611-106">Members</span></span>
|<span data-ttu-id="f1611-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f1611-107">Member</span></span>|<span data-ttu-id="f1611-108">値</span><span class="sxs-lookup"><span data-stu-id="f1611-108">Value</span></span>|<span data-ttu-id="f1611-109">説明</span><span class="sxs-lookup"><span data-stu-id="f1611-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1611-110">none</span><span class="sxs-lookup"><span data-stu-id="f1611-110">none</span></span>|<span data-ttu-id="f1611-111">0</span><span class="sxs-lookup"><span data-stu-id="f1611-111">0</span></span>|<span data-ttu-id="f1611-112">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="f1611-112">Not a valid action state</span></span>|
|<span data-ttu-id="f1611-113">保留中</span><span class="sxs-lookup"><span data-stu-id="f1611-113">pending</span></span>|<span data-ttu-id="f1611-114">1</span><span class="sxs-lookup"><span data-stu-id="f1611-114">1</span></span>|<span data-ttu-id="f1611-115">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="f1611-115">Action is pending</span></span>|
|<span data-ttu-id="f1611-116">キャンセル</span><span class="sxs-lookup"><span data-stu-id="f1611-116">canceled</span></span>|<span data-ttu-id="f1611-117">2</span><span class="sxs-lookup"><span data-stu-id="f1611-117">2</span></span>|<span data-ttu-id="f1611-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="f1611-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="f1611-119">アクティブです</span><span class="sxs-lookup"><span data-stu-id="f1611-119">active</span></span>|<span data-ttu-id="f1611-120">3</span><span class="sxs-lookup"><span data-stu-id="f1611-120">3</span></span>|<span data-ttu-id="f1611-121">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="f1611-121">Action is active.</span></span>|
|<span data-ttu-id="f1611-122">done</span><span class="sxs-lookup"><span data-stu-id="f1611-122">done</span></span>|<span data-ttu-id="f1611-123">4</span><span class="sxs-lookup"><span data-stu-id="f1611-123">4</span></span>|<span data-ttu-id="f1611-124">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="f1611-124">Action completed without errors.</span></span>|
|<span data-ttu-id="f1611-125">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f1611-125">failed</span></span>|<span data-ttu-id="f1611-126">5</span><span class="sxs-lookup"><span data-stu-id="f1611-126">5</span></span>|<span data-ttu-id="f1611-127">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="f1611-127">Action failed</span></span>|
|<span data-ttu-id="f1611-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="f1611-128">notSupported</span></span>|<span data-ttu-id="f1611-129">6</span><span class="sxs-lookup"><span data-stu-id="f1611-129">6</span></span>|<span data-ttu-id="f1611-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1611-130">Action is not supported.</span></span>|



