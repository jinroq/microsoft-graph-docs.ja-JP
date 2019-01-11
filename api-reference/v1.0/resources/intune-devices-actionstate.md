---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0c05e283b94473a5c8c43498ff5bf1dd82da7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871940"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fa592-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="fa592-103">actionState enum type</span></span>

> <span data-ttu-id="fa592-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa592-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa592-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="fa592-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="fa592-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="fa592-106">Members</span></span>
|<span data-ttu-id="fa592-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="fa592-107">Member</span></span>|<span data-ttu-id="fa592-108">値</span><span class="sxs-lookup"><span data-stu-id="fa592-108">Value</span></span>|<span data-ttu-id="fa592-109">説明</span><span class="sxs-lookup"><span data-stu-id="fa592-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa592-110">none</span><span class="sxs-lookup"><span data-stu-id="fa592-110">none</span></span>|<span data-ttu-id="fa592-111">0</span><span class="sxs-lookup"><span data-stu-id="fa592-111">0</span></span>|<span data-ttu-id="fa592-112">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="fa592-112">Not a valid action state</span></span>|
|<span data-ttu-id="fa592-113">保留中</span><span class="sxs-lookup"><span data-stu-id="fa592-113">pending</span></span>|<span data-ttu-id="fa592-114">1</span><span class="sxs-lookup"><span data-stu-id="fa592-114">1</span></span>|<span data-ttu-id="fa592-115">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="fa592-115">Action is pending</span></span>|
|<span data-ttu-id="fa592-116">キャンセル</span><span class="sxs-lookup"><span data-stu-id="fa592-116">canceled</span></span>|<span data-ttu-id="fa592-117">2</span><span class="sxs-lookup"><span data-stu-id="fa592-117">2</span></span>|<span data-ttu-id="fa592-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="fa592-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="fa592-119">アクティブです</span><span class="sxs-lookup"><span data-stu-id="fa592-119">active</span></span>|<span data-ttu-id="fa592-120">3</span><span class="sxs-lookup"><span data-stu-id="fa592-120">3</span></span>|<span data-ttu-id="fa592-121">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="fa592-121">Action is active.</span></span>|
|<span data-ttu-id="fa592-122">done</span><span class="sxs-lookup"><span data-stu-id="fa592-122">done</span></span>|<span data-ttu-id="fa592-123">4</span><span class="sxs-lookup"><span data-stu-id="fa592-123">4</span></span>|<span data-ttu-id="fa592-124">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="fa592-124">Action completed without errors.</span></span>|
|<span data-ttu-id="fa592-125">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="fa592-125">failed</span></span>|<span data-ttu-id="fa592-126">5</span><span class="sxs-lookup"><span data-stu-id="fa592-126">5</span></span>|<span data-ttu-id="fa592-127">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="fa592-127">Action failed</span></span>|
|<span data-ttu-id="fa592-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="fa592-128">notSupported</span></span>|<span data-ttu-id="fa592-129">6</span><span class="sxs-lookup"><span data-stu-id="fa592-129">6</span></span>|<span data-ttu-id="fa592-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa592-130">Action is not supported.</span></span>|



