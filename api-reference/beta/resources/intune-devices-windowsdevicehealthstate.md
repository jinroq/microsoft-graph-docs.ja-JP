---
title: windowsDeviceHealthState 列挙型
description: コンピューターエンドポイントの保護の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6086dc05d204e4c9cb23c77f79f98c3a207de35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941892"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="a6baa-103">windowsDeviceHealthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="a6baa-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="a6baa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6baa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6baa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6baa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6baa-106">コンピューターエンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="a6baa-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="a6baa-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6baa-107">Members</span></span>
|<span data-ttu-id="a6baa-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6baa-108">Member</span></span>|<span data-ttu-id="a6baa-109">値</span><span class="sxs-lookup"><span data-stu-id="a6baa-109">Value</span></span>|<span data-ttu-id="a6baa-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6baa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6baa-111">汚れ</span><span class="sxs-lookup"><span data-stu-id="a6baa-111">clean</span></span>|<span data-ttu-id="a6baa-112">.0</span><span class="sxs-lookup"><span data-stu-id="a6baa-112">0</span></span>|<span data-ttu-id="a6baa-113">コンピューターがクリーンであり、アクションは必要ありません</span><span class="sxs-lookup"><span data-stu-id="a6baa-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="a6baa-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="a6baa-114">fullScanPending</span></span>|<span data-ttu-id="a6baa-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a6baa-115">1</span></span>|<span data-ttu-id="a6baa-116">コンピューターが保留中の完全なスキャン状態である</span><span class="sxs-lookup"><span data-stu-id="a6baa-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="a6baa-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="a6baa-117">rebootPending</span></span>|<span data-ttu-id="a6baa-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a6baa-118">2</span></span>|<span data-ttu-id="a6baa-119">コンピューターが再起動の保留状態になっている</span><span class="sxs-lookup"><span data-stu-id="a6baa-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="a6baa-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="a6baa-120">manualStepsPending</span></span>|<span data-ttu-id="a6baa-121">2/4</span><span class="sxs-lookup"><span data-stu-id="a6baa-121">4</span></span>|<span data-ttu-id="a6baa-122">コンピューターが保留中の手動の手順状態である</span><span class="sxs-lookup"><span data-stu-id="a6baa-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="a6baa-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="a6baa-123">offlineScanPending</span></span>|<span data-ttu-id="a6baa-124">8 </span><span class="sxs-lookup"><span data-stu-id="a6baa-124">8</span></span>|<span data-ttu-id="a6baa-125">コンピューターが保留中のオフラインスキャン状態になっている</span><span class="sxs-lookup"><span data-stu-id="a6baa-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="a6baa-126">critical</span><span class="sxs-lookup"><span data-stu-id="a6baa-126">critical</span></span>|<span data-ttu-id="a6baa-127">16</span><span class="sxs-lookup"><span data-stu-id="a6baa-127">16</span></span>|<span data-ttu-id="a6baa-128">コンピューターは重大なエラー状態です</span><span class="sxs-lookup"><span data-stu-id="a6baa-128">Computer is in critical failure state</span></span>|




