---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d55ff0419c6178668bbee921c149c8bc797ebff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143401"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e9973-103">actionstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="e9973-103">actionState enum type</span></span>

> <span data-ttu-id="e9973-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9973-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9973-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9973-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9973-106">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="e9973-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="e9973-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9973-107">Members</span></span>
|<span data-ttu-id="e9973-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9973-108">Member</span></span>|<span data-ttu-id="e9973-109">値</span><span class="sxs-lookup"><span data-stu-id="e9973-109">Value</span></span>|<span data-ttu-id="e9973-110">説明</span><span class="sxs-lookup"><span data-stu-id="e9973-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9973-111">none</span><span class="sxs-lookup"><span data-stu-id="e9973-111">none</span></span>|<span data-ttu-id="e9973-112">.0</span><span class="sxs-lookup"><span data-stu-id="e9973-112">0</span></span>|<span data-ttu-id="e9973-113">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="e9973-113">Not a valid action state</span></span>|
|<span data-ttu-id="e9973-114">対する</span><span class="sxs-lookup"><span data-stu-id="e9973-114">pending</span></span>|<span data-ttu-id="e9973-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e9973-115">1</span></span>|<span data-ttu-id="e9973-116">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="e9973-116">Action is pending</span></span>|
|<span data-ttu-id="e9973-117">取り消す</span><span class="sxs-lookup"><span data-stu-id="e9973-117">canceled</span></span>|<span data-ttu-id="e9973-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e9973-118">2</span></span>|<span data-ttu-id="e9973-119">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="e9973-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="e9973-120">active</span><span class="sxs-lookup"><span data-stu-id="e9973-120">active</span></span>|<span data-ttu-id="e9973-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e9973-121">3</span></span>|<span data-ttu-id="e9973-122">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="e9973-122">Action is active.</span></span>|
|<span data-ttu-id="e9973-123">done</span><span class="sxs-lookup"><span data-stu-id="e9973-123">done</span></span>|<span data-ttu-id="e9973-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e9973-124">4</span></span>|<span data-ttu-id="e9973-125">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="e9973-125">Action completed without errors.</span></span>|
|<span data-ttu-id="e9973-126">フェール</span><span class="sxs-lookup"><span data-stu-id="e9973-126">failed</span></span>|<span data-ttu-id="e9973-127">5</span><span class="sxs-lookup"><span data-stu-id="e9973-127">5</span></span>|<span data-ttu-id="e9973-128">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="e9973-128">Action failed</span></span>|
|<span data-ttu-id="e9973-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="e9973-129">notSupported</span></span>|<span data-ttu-id="e9973-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e9973-130">6</span></span>|<span data-ttu-id="e9973-131">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9973-131">Action is not supported.</span></span>|




