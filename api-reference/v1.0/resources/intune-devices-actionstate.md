---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261489"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="2acb1-103">actionstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="2acb1-103">actionState enum type</span></span>

> <span data-ttu-id="2acb1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2acb1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2acb1-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="2acb1-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="2acb1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2acb1-106">Members</span></span>
|<span data-ttu-id="2acb1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2acb1-107">Member</span></span>|<span data-ttu-id="2acb1-108">値</span><span class="sxs-lookup"><span data-stu-id="2acb1-108">Value</span></span>|<span data-ttu-id="2acb1-109">説明</span><span class="sxs-lookup"><span data-stu-id="2acb1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2acb1-110">none</span><span class="sxs-lookup"><span data-stu-id="2acb1-110">none</span></span>|<span data-ttu-id="2acb1-111">.0</span><span class="sxs-lookup"><span data-stu-id="2acb1-111">0</span></span>|<span data-ttu-id="2acb1-112">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="2acb1-112">Not a valid action state</span></span>|
|<span data-ttu-id="2acb1-113">対する</span><span class="sxs-lookup"><span data-stu-id="2acb1-113">pending</span></span>|<span data-ttu-id="2acb1-114">1-d</span><span class="sxs-lookup"><span data-stu-id="2acb1-114">1</span></span>|<span data-ttu-id="2acb1-115">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="2acb1-115">Action is pending</span></span>|
|<span data-ttu-id="2acb1-116">取り消す</span><span class="sxs-lookup"><span data-stu-id="2acb1-116">canceled</span></span>|<span data-ttu-id="2acb1-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="2acb1-117">2</span></span>|<span data-ttu-id="2acb1-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="2acb1-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="2acb1-119">active</span><span class="sxs-lookup"><span data-stu-id="2acb1-119">active</span></span>|<span data-ttu-id="2acb1-120">1/3</span><span class="sxs-lookup"><span data-stu-id="2acb1-120">3</span></span>|<span data-ttu-id="2acb1-121">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="2acb1-121">Action is active.</span></span>|
|<span data-ttu-id="2acb1-122">done</span><span class="sxs-lookup"><span data-stu-id="2acb1-122">done</span></span>|<span data-ttu-id="2acb1-123">2/4</span><span class="sxs-lookup"><span data-stu-id="2acb1-123">4</span></span>|<span data-ttu-id="2acb1-124">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="2acb1-124">Action completed without errors.</span></span>|
|<span data-ttu-id="2acb1-125">フェール</span><span class="sxs-lookup"><span data-stu-id="2acb1-125">failed</span></span>|<span data-ttu-id="2acb1-126">5</span><span class="sxs-lookup"><span data-stu-id="2acb1-126">5</span></span>|<span data-ttu-id="2acb1-127">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="2acb1-127">Action failed</span></span>|
|<span data-ttu-id="2acb1-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="2acb1-128">notSupported</span></span>|<span data-ttu-id="2acb1-129">シックス</span><span class="sxs-lookup"><span data-stu-id="2acb1-129">6</span></span>|<span data-ttu-id="2acb1-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2acb1-130">Action is not supported.</span></span>|



