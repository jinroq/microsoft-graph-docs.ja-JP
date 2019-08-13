---
title: windowsDeviceHealthState 列挙型
description: コンピューターエンドポイントの保護の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b37f441a1ded71d3f299d6d38b58543aac130ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366455"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="c25f9-103">windowsDeviceHealthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="c25f9-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="c25f9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c25f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c25f9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c25f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c25f9-106">コンピューターエンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="c25f9-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="c25f9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c25f9-107">Members</span></span>
|<span data-ttu-id="c25f9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c25f9-108">Member</span></span>|<span data-ttu-id="c25f9-109">値</span><span class="sxs-lookup"><span data-stu-id="c25f9-109">Value</span></span>|<span data-ttu-id="c25f9-110">説明</span><span class="sxs-lookup"><span data-stu-id="c25f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c25f9-111">汚れ</span><span class="sxs-lookup"><span data-stu-id="c25f9-111">clean</span></span>|<span data-ttu-id="c25f9-112">.0</span><span class="sxs-lookup"><span data-stu-id="c25f9-112">0</span></span>|<span data-ttu-id="c25f9-113">コンピューターがクリーンであり、アクションは必要ありません</span><span class="sxs-lookup"><span data-stu-id="c25f9-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="c25f9-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="c25f9-114">fullScanPending</span></span>|<span data-ttu-id="c25f9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c25f9-115">1</span></span>|<span data-ttu-id="c25f9-116">コンピューターが保留中の完全なスキャン状態である</span><span class="sxs-lookup"><span data-stu-id="c25f9-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="c25f9-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="c25f9-117">rebootPending</span></span>|<span data-ttu-id="c25f9-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c25f9-118">2</span></span>|<span data-ttu-id="c25f9-119">コンピューターが再起動の保留状態になっている</span><span class="sxs-lookup"><span data-stu-id="c25f9-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="c25f9-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="c25f9-120">manualStepsPending</span></span>|<span data-ttu-id="c25f9-121">2/4</span><span class="sxs-lookup"><span data-stu-id="c25f9-121">4</span></span>|<span data-ttu-id="c25f9-122">コンピューターが保留中の手動の手順状態である</span><span class="sxs-lookup"><span data-stu-id="c25f9-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="c25f9-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="c25f9-123">offlineScanPending</span></span>|<span data-ttu-id="c25f9-124">8 </span><span class="sxs-lookup"><span data-stu-id="c25f9-124">8</span></span>|<span data-ttu-id="c25f9-125">コンピューターが保留中のオフラインスキャン状態になっている</span><span class="sxs-lookup"><span data-stu-id="c25f9-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="c25f9-126">critical</span><span class="sxs-lookup"><span data-stu-id="c25f9-126">critical</span></span>|<span data-ttu-id="c25f9-127">16</span><span class="sxs-lookup"><span data-stu-id="c25f9-127">16</span></span>|<span data-ttu-id="c25f9-128">コンピューターは重大なエラー状態です</span><span class="sxs-lookup"><span data-stu-id="c25f9-128">Computer is in critical failure state</span></span>|



