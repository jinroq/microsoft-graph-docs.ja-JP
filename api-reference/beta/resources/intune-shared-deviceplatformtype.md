---
title: devicePlatformType 列挙型
description: サポートされているプラットフォームの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a8c2f16f4adf4aa8dd9971f970b4af45fb320f4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341992"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="6fd70-103">devicePlatformType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6fd70-103">devicePlatformType enum type</span></span>

> <span data-ttu-id="6fd70-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fd70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fd70-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6fd70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fd70-106">サポートされているプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="6fd70-106">Supported platform types.</span></span>

## <a name="members"></a><span data-ttu-id="6fd70-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6fd70-107">Members</span></span>
|<span data-ttu-id="6fd70-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6fd70-108">Member</span></span>|<span data-ttu-id="6fd70-109">値</span><span class="sxs-lookup"><span data-stu-id="6fd70-109">Value</span></span>|<span data-ttu-id="6fd70-110">説明</span><span class="sxs-lookup"><span data-stu-id="6fd70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fd70-111">android</span><span class="sxs-lookup"><span data-stu-id="6fd70-111">android</span></span>|<span data-ttu-id="6fd70-112">.0</span><span class="sxs-lookup"><span data-stu-id="6fd70-112">0</span></span>|<span data-ttu-id="6fd70-113">Android.</span><span class="sxs-lookup"><span data-stu-id="6fd70-113">Android.</span></span>|
|<span data-ttu-id="6fd70-114">androidForWork</span><span class="sxs-lookup"><span data-stu-id="6fd70-114">androidForWork</span></span>|<span data-ttu-id="6fd70-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6fd70-115">1</span></span>|<span data-ttu-id="6fd70-116">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="6fd70-116">AndroidForWork.</span></span>|
|<span data-ttu-id="6fd70-117">iOS</span><span class="sxs-lookup"><span data-stu-id="6fd70-117">iOS</span></span>|<span data-ttu-id="6fd70-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6fd70-118">2</span></span>|<span data-ttu-id="6fd70-119">iOS.</span><span class="sxs-lookup"><span data-stu-id="6fd70-119">iOS.</span></span>|
|<span data-ttu-id="6fd70-120">macOS</span><span class="sxs-lookup"><span data-stu-id="6fd70-120">macOS</span></span>|<span data-ttu-id="6fd70-121">1/3</span><span class="sxs-lookup"><span data-stu-id="6fd70-121">3</span></span>|<span data-ttu-id="6fd70-122">MacOS.</span><span class="sxs-lookup"><span data-stu-id="6fd70-122">MacOS.</span></span>|
|<span data-ttu-id="6fd70-123">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="6fd70-123">windowsPhone81</span></span>|<span data-ttu-id="6fd70-124">2/4</span><span class="sxs-lookup"><span data-stu-id="6fd70-124">4</span></span>|<span data-ttu-id="6fd70-125">WindowsPhone 8.1</span><span class="sxs-lookup"><span data-stu-id="6fd70-125">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="6fd70-126">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="6fd70-126">windows81AndLater</span></span>|<span data-ttu-id="6fd70-127">5</span><span class="sxs-lookup"><span data-stu-id="6fd70-127">5</span></span>|<span data-ttu-id="6fd70-128">Windows 8.1 以降</span><span class="sxs-lookup"><span data-stu-id="6fd70-128">Windows 8.1 and later</span></span>|
|<span data-ttu-id="6fd70-129">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="6fd70-129">windows10AndLater</span></span>|<span data-ttu-id="6fd70-130">シックス</span><span class="sxs-lookup"><span data-stu-id="6fd70-130">6</span></span>|<span data-ttu-id="6fd70-131">Windows 10 以降。</span><span class="sxs-lookup"><span data-stu-id="6fd70-131">Windows 10 and later.</span></span>|
|<span data-ttu-id="6fd70-132">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="6fd70-132">androidWorkProfile</span></span>|<span data-ttu-id="6fd70-133">7</span><span class="sxs-lookup"><span data-stu-id="6fd70-133">7</span></span>|<span data-ttu-id="6fd70-134">Android の作業プロファイル。</span><span class="sxs-lookup"><span data-stu-id="6fd70-134">Android Work Profile.</span></span>|
|<span data-ttu-id="6fd70-135">不明</span><span class="sxs-lookup"><span data-stu-id="6fd70-135">unknown</span></span>|<span data-ttu-id="6fd70-136">8 </span><span class="sxs-lookup"><span data-stu-id="6fd70-136">8</span></span>|<span data-ttu-id="6fd70-137">わかり.</span><span class="sxs-lookup"><span data-stu-id="6fd70-137">Unknown.</span></span>|



