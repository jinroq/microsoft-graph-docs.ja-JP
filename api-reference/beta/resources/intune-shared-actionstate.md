---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793463"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="952f0-103">actionstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="952f0-103">actionState enum type</span></span>

> <span data-ttu-id="952f0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="952f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="952f0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="952f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="952f0-106">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="952f0-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="952f0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="952f0-107">Members</span></span>
|<span data-ttu-id="952f0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="952f0-108">Member</span></span>|<span data-ttu-id="952f0-109">値</span><span class="sxs-lookup"><span data-stu-id="952f0-109">Value</span></span>|<span data-ttu-id="952f0-110">説明</span><span class="sxs-lookup"><span data-stu-id="952f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="952f0-111">none</span><span class="sxs-lookup"><span data-stu-id="952f0-111">none</span></span>|<span data-ttu-id="952f0-112">.0</span><span class="sxs-lookup"><span data-stu-id="952f0-112">0</span></span>|<span data-ttu-id="952f0-113">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="952f0-113">Not a valid action state</span></span>|
|<span data-ttu-id="952f0-114">対する</span><span class="sxs-lookup"><span data-stu-id="952f0-114">pending</span></span>|<span data-ttu-id="952f0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="952f0-115">1</span></span>|<span data-ttu-id="952f0-116">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="952f0-116">Action is pending</span></span>|
|<span data-ttu-id="952f0-117">取り消す</span><span class="sxs-lookup"><span data-stu-id="952f0-117">canceled</span></span>|<span data-ttu-id="952f0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="952f0-118">2</span></span>|<span data-ttu-id="952f0-119">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="952f0-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="952f0-120">active</span><span class="sxs-lookup"><span data-stu-id="952f0-120">active</span></span>|<span data-ttu-id="952f0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="952f0-121">3</span></span>|<span data-ttu-id="952f0-122">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="952f0-122">Action is active.</span></span>|
|<span data-ttu-id="952f0-123">done</span><span class="sxs-lookup"><span data-stu-id="952f0-123">done</span></span>|<span data-ttu-id="952f0-124">2/4</span><span class="sxs-lookup"><span data-stu-id="952f0-124">4</span></span>|<span data-ttu-id="952f0-125">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="952f0-125">Action completed without errors.</span></span>|
|<span data-ttu-id="952f0-126">フェール</span><span class="sxs-lookup"><span data-stu-id="952f0-126">failed</span></span>|<span data-ttu-id="952f0-127">5</span><span class="sxs-lookup"><span data-stu-id="952f0-127">5</span></span>|<span data-ttu-id="952f0-128">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="952f0-128">Action failed</span></span>|
|<span data-ttu-id="952f0-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="952f0-129">notSupported</span></span>|<span data-ttu-id="952f0-130">シックス</span><span class="sxs-lookup"><span data-stu-id="952f0-130">6</span></span>|<span data-ttu-id="952f0-131">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="952f0-131">Action is not supported.</span></span>|





