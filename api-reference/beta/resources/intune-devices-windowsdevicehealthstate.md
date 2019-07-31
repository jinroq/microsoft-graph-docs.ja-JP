---
title: windowsDeviceHealthState 列挙型
description: コンピューターエンドポイントの保護の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a12ac4e09981e21b51d97109f72569cafe628ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999608"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="0b525-103">windowsDeviceHealthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="0b525-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="0b525-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b525-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b525-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b525-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b525-106">コンピューターエンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="0b525-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="0b525-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b525-107">Members</span></span>
|<span data-ttu-id="0b525-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b525-108">Member</span></span>|<span data-ttu-id="0b525-109">値</span><span class="sxs-lookup"><span data-stu-id="0b525-109">Value</span></span>|<span data-ttu-id="0b525-110">説明</span><span class="sxs-lookup"><span data-stu-id="0b525-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b525-111">汚れ</span><span class="sxs-lookup"><span data-stu-id="0b525-111">clean</span></span>|<span data-ttu-id="0b525-112">.0</span><span class="sxs-lookup"><span data-stu-id="0b525-112">0</span></span>|<span data-ttu-id="0b525-113">コンピューターがクリーンであり、アクションは必要ありません</span><span class="sxs-lookup"><span data-stu-id="0b525-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="0b525-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="0b525-114">fullScanPending</span></span>|<span data-ttu-id="0b525-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0b525-115">1</span></span>|<span data-ttu-id="0b525-116">コンピューターが保留中の完全なスキャン状態である</span><span class="sxs-lookup"><span data-stu-id="0b525-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="0b525-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="0b525-117">rebootPending</span></span>|<span data-ttu-id="0b525-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0b525-118">2</span></span>|<span data-ttu-id="0b525-119">コンピューターが再起動の保留状態になっている</span><span class="sxs-lookup"><span data-stu-id="0b525-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="0b525-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="0b525-120">manualStepsPending</span></span>|<span data-ttu-id="0b525-121">2/4</span><span class="sxs-lookup"><span data-stu-id="0b525-121">4</span></span>|<span data-ttu-id="0b525-122">コンピューターが保留中の手動の手順状態である</span><span class="sxs-lookup"><span data-stu-id="0b525-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="0b525-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="0b525-123">offlineScanPending</span></span>|<span data-ttu-id="0b525-124">8 </span><span class="sxs-lookup"><span data-stu-id="0b525-124">8</span></span>|<span data-ttu-id="0b525-125">コンピューターが保留中のオフラインスキャン状態になっている</span><span class="sxs-lookup"><span data-stu-id="0b525-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="0b525-126">critical</span><span class="sxs-lookup"><span data-stu-id="0b525-126">critical</span></span>|<span data-ttu-id="0b525-127">16</span><span class="sxs-lookup"><span data-stu-id="0b525-127">16</span></span>|<span data-ttu-id="0b525-128">コンピューターは重大なエラー状態です</span><span class="sxs-lookup"><span data-stu-id="0b525-128">Computer is in critical failure state</span></span>|





