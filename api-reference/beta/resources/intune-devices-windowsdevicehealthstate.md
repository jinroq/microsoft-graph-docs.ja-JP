---
title: windowsdevicehealthstate 列挙型
description: コンピューターエンドポイントの保護の状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156169"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="274d1-103">windowsdevicehealthstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="274d1-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="274d1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="274d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="274d1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="274d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="274d1-106">コンピューターエンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="274d1-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="274d1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="274d1-107">Members</span></span>
|<span data-ttu-id="274d1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="274d1-108">Member</span></span>|<span data-ttu-id="274d1-109">値</span><span class="sxs-lookup"><span data-stu-id="274d1-109">Value</span></span>|<span data-ttu-id="274d1-110">説明</span><span class="sxs-lookup"><span data-stu-id="274d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="274d1-111">クリーン</span><span class="sxs-lookup"><span data-stu-id="274d1-111">clean</span></span>|<span data-ttu-id="274d1-112">.0</span><span class="sxs-lookup"><span data-stu-id="274d1-112">0</span></span>|<span data-ttu-id="274d1-113">コンピューターがクリーンであり、アクションは必要ありません</span><span class="sxs-lookup"><span data-stu-id="274d1-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="274d1-114">fullscanpending</span><span class="sxs-lookup"><span data-stu-id="274d1-114">fullScanPending</span></span>|<span data-ttu-id="274d1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="274d1-115">1</span></span>|<span data-ttu-id="274d1-116">コンピューターが保留中の完全なスキャン状態である</span><span class="sxs-lookup"><span data-stu-id="274d1-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="274d1-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="274d1-117">rebootPending</span></span>|<span data-ttu-id="274d1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="274d1-118">2</span></span>|<span data-ttu-id="274d1-119">コンピューターが再起動の保留状態になっている</span><span class="sxs-lookup"><span data-stu-id="274d1-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="274d1-120">manualstepspending</span><span class="sxs-lookup"><span data-stu-id="274d1-120">manualStepsPending</span></span>|<span data-ttu-id="274d1-121">2/4</span><span class="sxs-lookup"><span data-stu-id="274d1-121">4</span></span>|<span data-ttu-id="274d1-122">コンピューターが保留中の手動の手順状態である</span><span class="sxs-lookup"><span data-stu-id="274d1-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="274d1-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="274d1-123">offlineScanPending</span></span>|<span data-ttu-id="274d1-124">~</span><span class="sxs-lookup"><span data-stu-id="274d1-124">8</span></span>|<span data-ttu-id="274d1-125">コンピューターが保留中のオフラインスキャン状態になっている</span><span class="sxs-lookup"><span data-stu-id="274d1-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="274d1-126">critical</span><span class="sxs-lookup"><span data-stu-id="274d1-126">critical</span></span>|<span data-ttu-id="274d1-127">16</span><span class="sxs-lookup"><span data-stu-id="274d1-127">16</span></span>|<span data-ttu-id="274d1-128">コンピューターは重大なエラー状態です</span><span class="sxs-lookup"><span data-stu-id="274d1-128">Computer is in critical failure state</span></span>|




