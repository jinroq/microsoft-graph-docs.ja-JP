---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c561f3ea046423e26daeb544d92b89a98e4bc55b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967519"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="601bc-103">actionState 列挙型</span><span class="sxs-lookup"><span data-stu-id="601bc-103">actionState enum type</span></span>

> <span data-ttu-id="601bc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="601bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="601bc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="601bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="601bc-106">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="601bc-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="601bc-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="601bc-107">Members</span></span>
|<span data-ttu-id="601bc-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="601bc-108">Member</span></span>|<span data-ttu-id="601bc-109">値</span><span class="sxs-lookup"><span data-stu-id="601bc-109">Value</span></span>|<span data-ttu-id="601bc-110">説明</span><span class="sxs-lookup"><span data-stu-id="601bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="601bc-111">none</span><span class="sxs-lookup"><span data-stu-id="601bc-111">none</span></span>|<span data-ttu-id="601bc-112">.0</span><span class="sxs-lookup"><span data-stu-id="601bc-112">0</span></span>|<span data-ttu-id="601bc-113">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="601bc-113">Not a valid action state</span></span>|
|<span data-ttu-id="601bc-114">対する</span><span class="sxs-lookup"><span data-stu-id="601bc-114">pending</span></span>|<span data-ttu-id="601bc-115">1-d</span><span class="sxs-lookup"><span data-stu-id="601bc-115">1</span></span>|<span data-ttu-id="601bc-116">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="601bc-116">Action is pending</span></span>|
|<span data-ttu-id="601bc-117">取り消す</span><span class="sxs-lookup"><span data-stu-id="601bc-117">canceled</span></span>|<span data-ttu-id="601bc-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="601bc-118">2</span></span>|<span data-ttu-id="601bc-119">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="601bc-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="601bc-120">active</span><span class="sxs-lookup"><span data-stu-id="601bc-120">active</span></span>|<span data-ttu-id="601bc-121">1/3</span><span class="sxs-lookup"><span data-stu-id="601bc-121">3</span></span>|<span data-ttu-id="601bc-122">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="601bc-122">Action is active.</span></span>|
|<span data-ttu-id="601bc-123">done</span><span class="sxs-lookup"><span data-stu-id="601bc-123">done</span></span>|<span data-ttu-id="601bc-124">2/4</span><span class="sxs-lookup"><span data-stu-id="601bc-124">4</span></span>|<span data-ttu-id="601bc-125">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="601bc-125">Action completed without errors.</span></span>|
|<span data-ttu-id="601bc-126">フェール</span><span class="sxs-lookup"><span data-stu-id="601bc-126">failed</span></span>|<span data-ttu-id="601bc-127">5</span><span class="sxs-lookup"><span data-stu-id="601bc-127">5</span></span>|<span data-ttu-id="601bc-128">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="601bc-128">Action failed</span></span>|
|<span data-ttu-id="601bc-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="601bc-129">notSupported</span></span>|<span data-ttu-id="601bc-130">シックス</span><span class="sxs-lookup"><span data-stu-id="601bc-130">6</span></span>|<span data-ttu-id="601bc-131">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="601bc-131">Action is not supported.</span></span>|





