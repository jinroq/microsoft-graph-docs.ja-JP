---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa3e3dcd9b563301fb87b9bae0f3c2957631334b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939918"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="db2db-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="db2db-103">actionState enum type</span></span>

> <span data-ttu-id="db2db-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db2db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db2db-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db2db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db2db-106">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="db2db-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="db2db-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="db2db-107">Members</span></span>
|<span data-ttu-id="db2db-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="db2db-108">Member</span></span>|<span data-ttu-id="db2db-109">値</span><span class="sxs-lookup"><span data-stu-id="db2db-109">Value</span></span>|<span data-ttu-id="db2db-110">説明</span><span class="sxs-lookup"><span data-stu-id="db2db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db2db-111">none</span><span class="sxs-lookup"><span data-stu-id="db2db-111">none</span></span>|<span data-ttu-id="db2db-112">.0</span><span class="sxs-lookup"><span data-stu-id="db2db-112">0</span></span>|<span data-ttu-id="db2db-113">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="db2db-113">Not a valid action state</span></span>|
|<span data-ttu-id="db2db-114">対する</span><span class="sxs-lookup"><span data-stu-id="db2db-114">pending</span></span>|<span data-ttu-id="db2db-115">1-d</span><span class="sxs-lookup"><span data-stu-id="db2db-115">1</span></span>|<span data-ttu-id="db2db-116">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="db2db-116">Action is pending</span></span>|
|<span data-ttu-id="db2db-117">取り消す</span><span class="sxs-lookup"><span data-stu-id="db2db-117">canceled</span></span>|<span data-ttu-id="db2db-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="db2db-118">2</span></span>|<span data-ttu-id="db2db-119">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="db2db-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="db2db-120">active</span><span class="sxs-lookup"><span data-stu-id="db2db-120">active</span></span>|<span data-ttu-id="db2db-121">1/3</span><span class="sxs-lookup"><span data-stu-id="db2db-121">3</span></span>|<span data-ttu-id="db2db-122">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="db2db-122">Action is active.</span></span>|
|<span data-ttu-id="db2db-123">done</span><span class="sxs-lookup"><span data-stu-id="db2db-123">done</span></span>|<span data-ttu-id="db2db-124">2/4</span><span class="sxs-lookup"><span data-stu-id="db2db-124">4</span></span>|<span data-ttu-id="db2db-125">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="db2db-125">Action completed without errors.</span></span>|
|<span data-ttu-id="db2db-126">フェール</span><span class="sxs-lookup"><span data-stu-id="db2db-126">failed</span></span>|<span data-ttu-id="db2db-127">5</span><span class="sxs-lookup"><span data-stu-id="db2db-127">5</span></span>|<span data-ttu-id="db2db-128">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="db2db-128">Action failed</span></span>|
|<span data-ttu-id="db2db-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="db2db-129">notSupported</span></span>|<span data-ttu-id="db2db-130">シックス</span><span class="sxs-lookup"><span data-stu-id="db2db-130">6</span></span>|<span data-ttu-id="db2db-131">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db2db-131">Action is not supported.</span></span>|




