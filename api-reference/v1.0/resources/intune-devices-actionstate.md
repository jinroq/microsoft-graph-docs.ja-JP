---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6be5ce422664d5666fd5c76c3ce51ad8a9d798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027518"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="d6d55-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6d55-103">actionState enum type</span></span>

> <span data-ttu-id="d6d55-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6d55-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d55-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="d6d55-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="d6d55-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6d55-106">Members</span></span>
|<span data-ttu-id="d6d55-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6d55-107">Member</span></span>|<span data-ttu-id="d6d55-108">値</span><span class="sxs-lookup"><span data-stu-id="d6d55-108">Value</span></span>|<span data-ttu-id="d6d55-109">説明</span><span class="sxs-lookup"><span data-stu-id="d6d55-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d55-110">none</span><span class="sxs-lookup"><span data-stu-id="d6d55-110">none</span></span>|<span data-ttu-id="d6d55-111">.0</span><span class="sxs-lookup"><span data-stu-id="d6d55-111">0</span></span>|<span data-ttu-id="d6d55-112">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="d6d55-112">Not a valid action state</span></span>|
|<span data-ttu-id="d6d55-113">対する</span><span class="sxs-lookup"><span data-stu-id="d6d55-113">pending</span></span>|<span data-ttu-id="d6d55-114">1-d</span><span class="sxs-lookup"><span data-stu-id="d6d55-114">1</span></span>|<span data-ttu-id="d6d55-115">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="d6d55-115">Action is pending</span></span>|
|<span data-ttu-id="d6d55-116">取り消す</span><span class="sxs-lookup"><span data-stu-id="d6d55-116">canceled</span></span>|<span data-ttu-id="d6d55-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d6d55-117">2</span></span>|<span data-ttu-id="d6d55-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="d6d55-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="d6d55-119">active</span><span class="sxs-lookup"><span data-stu-id="d6d55-119">active</span></span>|<span data-ttu-id="d6d55-120">1/3</span><span class="sxs-lookup"><span data-stu-id="d6d55-120">3</span></span>|<span data-ttu-id="d6d55-121">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="d6d55-121">Action is active.</span></span>|
|<span data-ttu-id="d6d55-122">done</span><span class="sxs-lookup"><span data-stu-id="d6d55-122">done</span></span>|<span data-ttu-id="d6d55-123">2/4</span><span class="sxs-lookup"><span data-stu-id="d6d55-123">4</span></span>|<span data-ttu-id="d6d55-124">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="d6d55-124">Action completed without errors.</span></span>|
|<span data-ttu-id="d6d55-125">フェール</span><span class="sxs-lookup"><span data-stu-id="d6d55-125">failed</span></span>|<span data-ttu-id="d6d55-126">5</span><span class="sxs-lookup"><span data-stu-id="d6d55-126">5</span></span>|<span data-ttu-id="d6d55-127">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="d6d55-127">Action failed</span></span>|
|<span data-ttu-id="d6d55-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="d6d55-128">notSupported</span></span>|<span data-ttu-id="d6d55-129">シックス</span><span class="sxs-lookup"><span data-stu-id="d6d55-129">6</span></span>|<span data-ttu-id="d6d55-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6d55-130">Action is not supported.</span></span>|



