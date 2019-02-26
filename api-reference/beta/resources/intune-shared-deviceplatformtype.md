---
title: devicePlatformType 列挙型
description: サポートされているプラットフォームの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e060cba22c0f5dcb45ab17f5624f7a0246123810
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139908"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="d353e-103">devicePlatformType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d353e-103">devicePlatformType enum type</span></span>

> <span data-ttu-id="d353e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d353e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d353e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d353e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d353e-106">サポートされているプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="d353e-106">Supported platform types.</span></span>

## <a name="members"></a><span data-ttu-id="d353e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d353e-107">Members</span></span>
|<span data-ttu-id="d353e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d353e-108">Member</span></span>|<span data-ttu-id="d353e-109">値</span><span class="sxs-lookup"><span data-stu-id="d353e-109">Value</span></span>|<span data-ttu-id="d353e-110">説明</span><span class="sxs-lookup"><span data-stu-id="d353e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d353e-111">android</span><span class="sxs-lookup"><span data-stu-id="d353e-111">android</span></span>|<span data-ttu-id="d353e-112">.0</span><span class="sxs-lookup"><span data-stu-id="d353e-112">0</span></span>|<span data-ttu-id="d353e-113">Android.</span><span class="sxs-lookup"><span data-stu-id="d353e-113">Android.</span></span>|
|<span data-ttu-id="d353e-114">androidforwork</span><span class="sxs-lookup"><span data-stu-id="d353e-114">androidForWork</span></span>|<span data-ttu-id="d353e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d353e-115">1</span></span>|<span data-ttu-id="d353e-116">androidforwork。</span><span class="sxs-lookup"><span data-stu-id="d353e-116">AndroidForWork.</span></span>|
|<span data-ttu-id="d353e-117">iOS</span><span class="sxs-lookup"><span data-stu-id="d353e-117">iOS</span></span>|<span data-ttu-id="d353e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d353e-118">2</span></span>|<span data-ttu-id="d353e-119">iOS.</span><span class="sxs-lookup"><span data-stu-id="d353e-119">iOS.</span></span>|
|<span data-ttu-id="d353e-120">macOS</span><span class="sxs-lookup"><span data-stu-id="d353e-120">macOS</span></span>|<span data-ttu-id="d353e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d353e-121">3</span></span>|<span data-ttu-id="d353e-122">MacOS.</span><span class="sxs-lookup"><span data-stu-id="d353e-122">MacOS.</span></span>|
|<span data-ttu-id="d353e-123">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="d353e-123">windowsPhone81</span></span>|<span data-ttu-id="d353e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d353e-124">4</span></span>|<span data-ttu-id="d353e-125">WindowsPhone 8.1</span><span class="sxs-lookup"><span data-stu-id="d353e-125">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="d353e-126">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="d353e-126">windows81AndLater</span></span>|<span data-ttu-id="d353e-127">5</span><span class="sxs-lookup"><span data-stu-id="d353e-127">5</span></span>|<span data-ttu-id="d353e-128">Windows 8.1 以降</span><span class="sxs-lookup"><span data-stu-id="d353e-128">Windows 8.1 and later</span></span>|
|<span data-ttu-id="d353e-129">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="d353e-129">windows10AndLater</span></span>|<span data-ttu-id="d353e-130">シックス</span><span class="sxs-lookup"><span data-stu-id="d353e-130">6</span></span>|<span data-ttu-id="d353e-131">Windows 10 以降。</span><span class="sxs-lookup"><span data-stu-id="d353e-131">Windows 10 and later.</span></span>|
|<span data-ttu-id="d353e-132">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="d353e-132">androidWorkProfile</span></span>|<span data-ttu-id="d353e-133">7</span><span class="sxs-lookup"><span data-stu-id="d353e-133">7</span></span>|<span data-ttu-id="d353e-134">Android の作業プロファイル。</span><span class="sxs-lookup"><span data-stu-id="d353e-134">Android Work Profile.</span></span>|




