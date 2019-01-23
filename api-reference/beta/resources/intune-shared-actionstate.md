---
title: actionState 列挙型
description: デバイス上のアクションの状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421614"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="bc9eb-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="bc9eb-103">actionState enum type</span></span>

> <span data-ttu-id="bc9eb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc9eb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc9eb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc9eb-107">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="bc9eb-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="bc9eb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bc9eb-108">Members</span></span>
|<span data-ttu-id="bc9eb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="bc9eb-109">Member</span></span>|<span data-ttu-id="bc9eb-110">値</span><span class="sxs-lookup"><span data-stu-id="bc9eb-110">Value</span></span>|<span data-ttu-id="bc9eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="bc9eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc9eb-112">none</span><span class="sxs-lookup"><span data-stu-id="bc9eb-112">none</span></span>|<span data-ttu-id="bc9eb-113">0</span><span class="sxs-lookup"><span data-stu-id="bc9eb-113">0</span></span>|<span data-ttu-id="bc9eb-114">アクションが有効な状態ではなく</span><span class="sxs-lookup"><span data-stu-id="bc9eb-114">Not a valid action state</span></span>|
|<span data-ttu-id="bc9eb-115">保留中</span><span class="sxs-lookup"><span data-stu-id="bc9eb-115">pending</span></span>|<span data-ttu-id="bc9eb-116">1</span><span class="sxs-lookup"><span data-stu-id="bc9eb-116">1</span></span>|<span data-ttu-id="bc9eb-117">操作が保留中です。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-117">Action is pending</span></span>|
|<span data-ttu-id="bc9eb-118">キャンセル</span><span class="sxs-lookup"><span data-stu-id="bc9eb-118">canceled</span></span>|<span data-ttu-id="bc9eb-119">2</span><span class="sxs-lookup"><span data-stu-id="bc9eb-119">2</span></span>|<span data-ttu-id="bc9eb-120">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="bc9eb-121">アクティブです</span><span class="sxs-lookup"><span data-stu-id="bc9eb-121">active</span></span>|<span data-ttu-id="bc9eb-122">3</span><span class="sxs-lookup"><span data-stu-id="bc9eb-122">3</span></span>|<span data-ttu-id="bc9eb-123">影響はありません。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-123">Action is active.</span></span>|
|<span data-ttu-id="bc9eb-124">done</span><span class="sxs-lookup"><span data-stu-id="bc9eb-124">done</span></span>|<span data-ttu-id="bc9eb-125">4</span><span class="sxs-lookup"><span data-stu-id="bc9eb-125">4</span></span>|<span data-ttu-id="bc9eb-126">操作がエラーなく完了しました。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-126">Action completed without errors.</span></span>|
|<span data-ttu-id="bc9eb-127">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-127">failed</span></span>|<span data-ttu-id="bc9eb-128">5</span><span class="sxs-lookup"><span data-stu-id="bc9eb-128">5</span></span>|<span data-ttu-id="bc9eb-129">操作が失敗しました</span><span class="sxs-lookup"><span data-stu-id="bc9eb-129">Action failed</span></span>|
|<span data-ttu-id="bc9eb-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="bc9eb-130">notSupported</span></span>|<span data-ttu-id="bc9eb-131">6</span><span class="sxs-lookup"><span data-stu-id="bc9eb-131">6</span></span>|<span data-ttu-id="bc9eb-132">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc9eb-132">Action is not supported.</span></span>|




