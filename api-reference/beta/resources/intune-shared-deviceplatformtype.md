---
title: devicePlatformType 列挙型
description: プラットフォーム ・ タイプをサポートします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0927464dc16a7b2a0c2f1f580316c81774499287
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419787"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="3b9a1-103">devicePlatformType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3b9a1-103">devicePlatformType enum type</span></span>

> <span data-ttu-id="3b9a1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b9a1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b9a1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b9a1-107">プラットフォーム ・ タイプをサポートします。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-107">Supported platform types.</span></span>

## <a name="members"></a><span data-ttu-id="3b9a1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b9a1-108">Members</span></span>
|<span data-ttu-id="3b9a1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b9a1-109">Member</span></span>|<span data-ttu-id="3b9a1-110">値</span><span class="sxs-lookup"><span data-stu-id="3b9a1-110">Value</span></span>|<span data-ttu-id="3b9a1-111">説明</span><span class="sxs-lookup"><span data-stu-id="3b9a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b9a1-112">android</span><span class="sxs-lookup"><span data-stu-id="3b9a1-112">android</span></span>|<span data-ttu-id="3b9a1-113">0</span><span class="sxs-lookup"><span data-stu-id="3b9a1-113">0</span></span>|<span data-ttu-id="3b9a1-114">Android。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-114">Android.</span></span>|
|<span data-ttu-id="3b9a1-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="3b9a1-115">androidForWork</span></span>|<span data-ttu-id="3b9a1-116">1</span><span class="sxs-lookup"><span data-stu-id="3b9a1-116">1</span></span>|<span data-ttu-id="3b9a1-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-117">AndroidForWork.</span></span>|
|<span data-ttu-id="3b9a1-118">iOS</span><span class="sxs-lookup"><span data-stu-id="3b9a1-118">iOS</span></span>|<span data-ttu-id="3b9a1-119">2</span><span class="sxs-lookup"><span data-stu-id="3b9a1-119">2</span></span>|<span data-ttu-id="3b9a1-120">iOS です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-120">iOS.</span></span>|
|<span data-ttu-id="3b9a1-121">macOS</span><span class="sxs-lookup"><span data-stu-id="3b9a1-121">macOS</span></span>|<span data-ttu-id="3b9a1-122">3</span><span class="sxs-lookup"><span data-stu-id="3b9a1-122">3</span></span>|<span data-ttu-id="3b9a1-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-123">MacOS.</span></span>|
|<span data-ttu-id="3b9a1-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="3b9a1-124">windowsPhone81</span></span>|<span data-ttu-id="3b9a1-125">4</span><span class="sxs-lookup"><span data-stu-id="3b9a1-125">4</span></span>|<span data-ttu-id="3b9a1-126">WindowsPhone 8.1 です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="3b9a1-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="3b9a1-127">windows81AndLater</span></span>|<span data-ttu-id="3b9a1-128">5</span><span class="sxs-lookup"><span data-stu-id="3b9a1-128">5</span></span>|<span data-ttu-id="3b9a1-129">およびそれ以降の Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="3b9a1-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="3b9a1-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="3b9a1-130">windows10AndLater</span></span>|<span data-ttu-id="3b9a1-131">6</span><span class="sxs-lookup"><span data-stu-id="3b9a1-131">6</span></span>|<span data-ttu-id="3b9a1-132">Windows 10 以降です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="3b9a1-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="3b9a1-133">androidWorkProfile</span></span>|<span data-ttu-id="3b9a1-134">7</span><span class="sxs-lookup"><span data-stu-id="3b9a1-134">7</span></span>|<span data-ttu-id="3b9a1-135">Android 作業プロファイルです。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-135">Android Work Profile.</span></span>|




