---
title: deviceType 列挙型
description: デバイスの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e29fb236bbfeca914878e92d8b565502e5658f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525223"
---
# <a name="devicetype-enum-type"></a><span data-ttu-id="9e2c6-103">deviceType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9e2c6-103">deviceType enum type</span></span>

> <span data-ttu-id="9e2c6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e2c6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e2c6-106">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-106">Device type.</span></span>

## <a name="members"></a><span data-ttu-id="9e2c6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e2c6-107">Members</span></span>
|<span data-ttu-id="9e2c6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e2c6-108">Member</span></span>|<span data-ttu-id="9e2c6-109">値</span><span class="sxs-lookup"><span data-stu-id="9e2c6-109">Value</span></span>|<span data-ttu-id="9e2c6-110">説明</span><span class="sxs-lookup"><span data-stu-id="9e2c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2c6-111">コンピューター</span><span class="sxs-lookup"><span data-stu-id="9e2c6-111">desktop</span></span>|<span data-ttu-id="9e2c6-112">.0</span><span class="sxs-lookup"><span data-stu-id="9e2c6-112">0</span></span>|<span data-ttu-id="9e2c6-113">コンピューター.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-113">Desktop.</span></span>|
|<span data-ttu-id="9e2c6-114">windowsRT</span><span class="sxs-lookup"><span data-stu-id="9e2c6-114">windowsRT</span></span>|<span data-ttu-id="9e2c6-115">1 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-115">1</span></span>|<span data-ttu-id="9e2c6-116">WindowsRT。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-116">WindowsRT.</span></span>|
|<span data-ttu-id="9e2c6-117">winMO6</span><span class="sxs-lookup"><span data-stu-id="9e2c6-117">winMO6</span></span>|<span data-ttu-id="9e2c6-118">2 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-118">2</span></span>|<span data-ttu-id="9e2c6-119">WinMO6。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-119">WinMO6.</span></span>|
|<span data-ttu-id="9e2c6-120">nokia</span><span class="sxs-lookup"><span data-stu-id="9e2c6-120">nokia</span></span>|<span data-ttu-id="9e2c6-121">3 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-121">3</span></span>|<span data-ttu-id="9e2c6-122">Nokia.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-122">Nokia.</span></span>|
|<span data-ttu-id="9e2c6-123">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="9e2c6-123">windowsPhone</span></span>|<span data-ttu-id="9e2c6-124">4 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-124">4</span></span>|<span data-ttu-id="9e2c6-125">Windows phone。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-125">Windows phone.</span></span>|
|<span data-ttu-id="9e2c6-126">Mac</span><span class="sxs-lookup"><span data-stu-id="9e2c6-126">mac</span></span>|<span data-ttu-id="9e2c6-127">5 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-127">5</span></span>|<span data-ttu-id="9e2c6-128">Mac.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-128">Mac.</span></span>|
|<span data-ttu-id="9e2c6-129">win</span><span class="sxs-lookup"><span data-stu-id="9e2c6-129">winCE</span></span>|<span data-ttu-id="9e2c6-130">6 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-130">6</span></span>|<span data-ttu-id="9e2c6-131">win.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-131">WinCE.</span></span>|
|<span data-ttu-id="9e2c6-132">winembedded</span><span class="sxs-lookup"><span data-stu-id="9e2c6-132">winEmbedded</span></span>|<span data-ttu-id="9e2c6-133">7 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-133">7</span></span>|<span data-ttu-id="9e2c6-134">winembedded。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-134">WinEmbedded.</span></span>|
|<span data-ttu-id="9e2c6-135">iPhone</span><span class="sxs-lookup"><span data-stu-id="9e2c6-135">iPhone</span></span>|<span data-ttu-id="9e2c6-136">8 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-136">8</span></span>|<span data-ttu-id="9e2c6-137">iPhone.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-137">iPhone.</span></span>|
|<span data-ttu-id="9e2c6-138">iPad</span><span class="sxs-lookup"><span data-stu-id="9e2c6-138">iPad</span></span>|<span data-ttu-id="9e2c6-139">9 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-139">9</span></span>|<span data-ttu-id="9e2c6-140">iPad.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-140">iPad.</span></span>|
|<span data-ttu-id="9e2c6-141">iPod</span><span class="sxs-lookup"><span data-stu-id="9e2c6-141">iPod</span></span>|<span data-ttu-id="9e2c6-142">10  </span><span class="sxs-lookup"><span data-stu-id="9e2c6-142">10</span></span>|<span data-ttu-id="9e2c6-143">iPodTouch。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-143">iPodTouch.</span></span>|
|<span data-ttu-id="9e2c6-144">android</span><span class="sxs-lookup"><span data-stu-id="9e2c6-144">android</span></span>|<span data-ttu-id="9e2c6-145">11 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-145">11</span></span>|<span data-ttu-id="9e2c6-146">Android.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-146">Android.</span></span>|
|<span data-ttu-id="9e2c6-147">iソケットコンシューマー</span><span class="sxs-lookup"><span data-stu-id="9e2c6-147">iSocConsumer</span></span>|<span data-ttu-id="9e2c6-148">12 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-148">12</span></span>|<span data-ttu-id="9e2c6-149">iソケットコンシューマー。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-149">iSocConsumer.</span></span>|
|<span data-ttu-id="9e2c6-150">unix</span><span class="sxs-lookup"><span data-stu-id="9e2c6-150">unix</span></span>|<span data-ttu-id="9e2c6-151">13 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-151">13</span></span>|<span data-ttu-id="9e2c6-152">Unix.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-152">Unix.</span></span>|
|<span data-ttu-id="9e2c6-153">macmdm</span><span class="sxs-lookup"><span data-stu-id="9e2c6-153">macMDM</span></span>|<span data-ttu-id="9e2c6-154">14 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-154">14</span></span>|<span data-ttu-id="9e2c6-155">MDM エージェントが組み込まれている Mac OS X クライアント。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-155">Mac OS X client using built in MDM agent.</span></span>|
|<span data-ttu-id="9e2c6-156">holoLens</span><span class="sxs-lookup"><span data-stu-id="9e2c6-156">holoLens</span></span>|<span data-ttu-id="9e2c6-157">15 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-157">15</span></span>|<span data-ttu-id="9e2c6-158">凝った Windows 10 goggles を表します。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-158">Representing the fancy Windows 10 goggles.</span></span>|
|<span data-ttu-id="9e2c6-159">surfaceHub</span><span class="sxs-lookup"><span data-stu-id="9e2c6-159">surfaceHub</span></span>|<span data-ttu-id="9e2c6-160">16 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-160">16</span></span>|<span data-ttu-id="9e2c6-161">Surface HUB デバイス。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-161">Surface HUB device.</span></span>|
|<span data-ttu-id="9e2c6-162">androidforwork</span><span class="sxs-lookup"><span data-stu-id="9e2c6-162">androidForWork</span></span>|<span data-ttu-id="9e2c6-163">17 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-163">17</span></span>|<span data-ttu-id="9e2c6-164">Android for work デバイス。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-164">Android for work device.</span></span>|
|<span data-ttu-id="9e2c6-165">androidenterprise</span><span class="sxs-lookup"><span data-stu-id="9e2c6-165">androidEnterprise</span></span>|<span data-ttu-id="9e2c6-166">18 </span><span class="sxs-lookup"><span data-stu-id="9e2c6-166">18</span></span>|<span data-ttu-id="9e2c6-167">Android エンタープライズデバイス。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-167">Android enterprise device.</span></span>|
|<span data-ttu-id="9e2c6-168">blackberry</span><span class="sxs-lookup"><span data-stu-id="9e2c6-168">blackberry</span></span>|<span data-ttu-id="9e2c6-169">100</span><span class="sxs-lookup"><span data-stu-id="9e2c6-169">100</span></span>|<span data-ttu-id="9e2c6-170">Blackberry.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-170">Blackberry.</span></span>|
|<span data-ttu-id="9e2c6-171">ヤシ</span><span class="sxs-lookup"><span data-stu-id="9e2c6-171">palm</span></span>|<span data-ttu-id="9e2c6-172">101</span><span class="sxs-lookup"><span data-stu-id="9e2c6-172">101</span></span>|<span data-ttu-id="9e2c6-173">ヤシ.</span><span class="sxs-lookup"><span data-stu-id="9e2c6-173">Palm.</span></span>|
|<span data-ttu-id="9e2c6-174">不明</span><span class="sxs-lookup"><span data-stu-id="9e2c6-174">unknown</span></span>|<span data-ttu-id="9e2c6-175">255</span><span class="sxs-lookup"><span data-stu-id="9e2c6-175">255</span></span>|<span data-ttu-id="9e2c6-176">デバイスの種類が不明であることを表します。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-176">Represents that the device type is unknown.</span></span>|




