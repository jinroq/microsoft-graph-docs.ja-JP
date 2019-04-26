---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566319"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b821b-103">actionstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="b821b-103">actionState enum type</span></span>

> <span data-ttu-id="b821b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b821b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b821b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b821b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b821b-106">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="b821b-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="b821b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b821b-107">Members</span></span>
|<span data-ttu-id="b821b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b821b-108">Member</span></span>|<span data-ttu-id="b821b-109">値</span><span class="sxs-lookup"><span data-stu-id="b821b-109">Value</span></span>|<span data-ttu-id="b821b-110">説明</span><span class="sxs-lookup"><span data-stu-id="b821b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b821b-111">なし</span><span class="sxs-lookup"><span data-stu-id="b821b-111">none</span></span>|<span data-ttu-id="b821b-112">.0</span><span class="sxs-lookup"><span data-stu-id="b821b-112">0</span></span>|<span data-ttu-id="b821b-113">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="b821b-113">Not a valid action state</span></span>|
|<span data-ttu-id="b821b-114">対する</span><span class="sxs-lookup"><span data-stu-id="b821b-114">pending</span></span>|<span data-ttu-id="b821b-115">1 </span><span class="sxs-lookup"><span data-stu-id="b821b-115">1</span></span>|<span data-ttu-id="b821b-116">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="b821b-116">Action is pending</span></span>|
|<span data-ttu-id="b821b-117">取り消す</span><span class="sxs-lookup"><span data-stu-id="b821b-117">canceled</span></span>|<span data-ttu-id="b821b-118">2 </span><span class="sxs-lookup"><span data-stu-id="b821b-118">2</span></span>|<span data-ttu-id="b821b-119">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="b821b-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="b821b-120">active</span><span class="sxs-lookup"><span data-stu-id="b821b-120">active</span></span>|<span data-ttu-id="b821b-121">3 </span><span class="sxs-lookup"><span data-stu-id="b821b-121">3</span></span>|<span data-ttu-id="b821b-122">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="b821b-122">Action is active.</span></span>|
|<span data-ttu-id="b821b-123">done</span><span class="sxs-lookup"><span data-stu-id="b821b-123">done</span></span>|<span data-ttu-id="b821b-124">4 </span><span class="sxs-lookup"><span data-stu-id="b821b-124">4</span></span>|<span data-ttu-id="b821b-125">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="b821b-125">Action completed without errors.</span></span>|
|<span data-ttu-id="b821b-126">フェール</span><span class="sxs-lookup"><span data-stu-id="b821b-126">failed</span></span>|<span data-ttu-id="b821b-127">5 </span><span class="sxs-lookup"><span data-stu-id="b821b-127">5</span></span>|<span data-ttu-id="b821b-128">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="b821b-128">Action failed</span></span>|
|<span data-ttu-id="b821b-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="b821b-129">notSupported</span></span>|<span data-ttu-id="b821b-130">6 </span><span class="sxs-lookup"><span data-stu-id="b821b-130">6</span></span>|<span data-ttu-id="b821b-131">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b821b-131">Action is not supported.</span></span>|





