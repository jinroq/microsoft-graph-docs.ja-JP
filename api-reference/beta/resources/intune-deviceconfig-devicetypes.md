---
title: devicetypes 列挙型
description: デバイスの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 604009d8a636a367203f9c9ced69aa22f40bfbc7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567187"
---
# <a name="devicetypes-enum-type"></a><span data-ttu-id="40972-103">devicetypes 列挙型</span><span class="sxs-lookup"><span data-stu-id="40972-103">deviceTypes enum type</span></span>

> <span data-ttu-id="40972-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40972-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40972-106">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="40972-106">Device type.</span></span>

## <a name="members"></a><span data-ttu-id="40972-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="40972-107">Members</span></span>
|<span data-ttu-id="40972-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="40972-108">Member</span></span>|<span data-ttu-id="40972-109">値</span><span class="sxs-lookup"><span data-stu-id="40972-109">Value</span></span>|<span data-ttu-id="40972-110">説明</span><span class="sxs-lookup"><span data-stu-id="40972-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40972-111">コンピューター</span><span class="sxs-lookup"><span data-stu-id="40972-111">desktop</span></span>|<span data-ttu-id="40972-112">.0</span><span class="sxs-lookup"><span data-stu-id="40972-112">0</span></span>|<span data-ttu-id="40972-113">コンピューター.</span><span class="sxs-lookup"><span data-stu-id="40972-113">Desktop.</span></span>|
|<span data-ttu-id="40972-114">windowsRT</span><span class="sxs-lookup"><span data-stu-id="40972-114">windowsRT</span></span>|<span data-ttu-id="40972-115">1 </span><span class="sxs-lookup"><span data-stu-id="40972-115">1</span></span>|<span data-ttu-id="40972-116">WindowsRT。</span><span class="sxs-lookup"><span data-stu-id="40972-116">WindowsRT.</span></span>|
|<span data-ttu-id="40972-117">winMO6</span><span class="sxs-lookup"><span data-stu-id="40972-117">winMO6</span></span>|<span data-ttu-id="40972-118">2 </span><span class="sxs-lookup"><span data-stu-id="40972-118">2</span></span>|<span data-ttu-id="40972-119">WinMO6。</span><span class="sxs-lookup"><span data-stu-id="40972-119">WinMO6.</span></span>|
|<span data-ttu-id="40972-120">nokia</span><span class="sxs-lookup"><span data-stu-id="40972-120">nokia</span></span>|<span data-ttu-id="40972-121">3 </span><span class="sxs-lookup"><span data-stu-id="40972-121">3</span></span>|<span data-ttu-id="40972-122">Nokia.</span><span class="sxs-lookup"><span data-stu-id="40972-122">Nokia.</span></span>|
|<span data-ttu-id="40972-123">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="40972-123">windowsPhone</span></span>|<span data-ttu-id="40972-124">4 </span><span class="sxs-lookup"><span data-stu-id="40972-124">4</span></span>|<span data-ttu-id="40972-125">Windows phone。</span><span class="sxs-lookup"><span data-stu-id="40972-125">Windows phone.</span></span>|
|<span data-ttu-id="40972-126">Mac</span><span class="sxs-lookup"><span data-stu-id="40972-126">mac</span></span>|<span data-ttu-id="40972-127">5 </span><span class="sxs-lookup"><span data-stu-id="40972-127">5</span></span>|<span data-ttu-id="40972-128">Mac.</span><span class="sxs-lookup"><span data-stu-id="40972-128">Mac.</span></span>|
|<span data-ttu-id="40972-129">win</span><span class="sxs-lookup"><span data-stu-id="40972-129">winCE</span></span>|<span data-ttu-id="40972-130">6 </span><span class="sxs-lookup"><span data-stu-id="40972-130">6</span></span>|<span data-ttu-id="40972-131">win.</span><span class="sxs-lookup"><span data-stu-id="40972-131">WinCE.</span></span>|
|<span data-ttu-id="40972-132">winembedded</span><span class="sxs-lookup"><span data-stu-id="40972-132">winEmbedded</span></span>|<span data-ttu-id="40972-133">7 </span><span class="sxs-lookup"><span data-stu-id="40972-133">7</span></span>|<span data-ttu-id="40972-134">winembedded。</span><span class="sxs-lookup"><span data-stu-id="40972-134">WinEmbedded.</span></span>|
|<span data-ttu-id="40972-135">iPhone</span><span class="sxs-lookup"><span data-stu-id="40972-135">iPhone</span></span>|<span data-ttu-id="40972-136">8 </span><span class="sxs-lookup"><span data-stu-id="40972-136">8</span></span>|<span data-ttu-id="40972-137">iPhone.</span><span class="sxs-lookup"><span data-stu-id="40972-137">iPhone.</span></span>|
|<span data-ttu-id="40972-138">iPad</span><span class="sxs-lookup"><span data-stu-id="40972-138">iPad</span></span>|<span data-ttu-id="40972-139">9 </span><span class="sxs-lookup"><span data-stu-id="40972-139">9</span></span>|<span data-ttu-id="40972-140">iPad.</span><span class="sxs-lookup"><span data-stu-id="40972-140">iPad.</span></span>|
|<span data-ttu-id="40972-141">iPod</span><span class="sxs-lookup"><span data-stu-id="40972-141">iPod</span></span>|<span data-ttu-id="40972-142">10  </span><span class="sxs-lookup"><span data-stu-id="40972-142">10</span></span>|<span data-ttu-id="40972-143">iPodTouch。</span><span class="sxs-lookup"><span data-stu-id="40972-143">iPodTouch.</span></span>|
|<span data-ttu-id="40972-144">android</span><span class="sxs-lookup"><span data-stu-id="40972-144">android</span></span>|<span data-ttu-id="40972-145">11 </span><span class="sxs-lookup"><span data-stu-id="40972-145">11</span></span>|<span data-ttu-id="40972-146">Android.</span><span class="sxs-lookup"><span data-stu-id="40972-146">Android.</span></span>|
|<span data-ttu-id="40972-147">iソケットコンシューマー</span><span class="sxs-lookup"><span data-stu-id="40972-147">iSocConsumer</span></span>|<span data-ttu-id="40972-148">12 </span><span class="sxs-lookup"><span data-stu-id="40972-148">12</span></span>|<span data-ttu-id="40972-149">iソケットコンシューマー。</span><span class="sxs-lookup"><span data-stu-id="40972-149">iSocConsumer.</span></span>|
|<span data-ttu-id="40972-150">unix</span><span class="sxs-lookup"><span data-stu-id="40972-150">unix</span></span>|<span data-ttu-id="40972-151">13 </span><span class="sxs-lookup"><span data-stu-id="40972-151">13</span></span>|<span data-ttu-id="40972-152">Unix.</span><span class="sxs-lookup"><span data-stu-id="40972-152">Unix.</span></span>|
|<span data-ttu-id="40972-153">macmdm</span><span class="sxs-lookup"><span data-stu-id="40972-153">macMDM</span></span>|<span data-ttu-id="40972-154">14 </span><span class="sxs-lookup"><span data-stu-id="40972-154">14</span></span>|<span data-ttu-id="40972-155">MDM エージェントが組み込まれている Mac OS X クライアント。</span><span class="sxs-lookup"><span data-stu-id="40972-155">Mac OS X client using built in MDM agent.</span></span>|
|<span data-ttu-id="40972-156">holoLens</span><span class="sxs-lookup"><span data-stu-id="40972-156">holoLens</span></span>|<span data-ttu-id="40972-157">15 </span><span class="sxs-lookup"><span data-stu-id="40972-157">15</span></span>|<span data-ttu-id="40972-158">凝った Windows 10 goggles を表します。</span><span class="sxs-lookup"><span data-stu-id="40972-158">Representing the fancy Windows 10 goggles.</span></span>|
|<span data-ttu-id="40972-159">surfaceHub</span><span class="sxs-lookup"><span data-stu-id="40972-159">surfaceHub</span></span>|<span data-ttu-id="40972-160">16 </span><span class="sxs-lookup"><span data-stu-id="40972-160">16</span></span>|<span data-ttu-id="40972-161">Surface HUB デバイス。</span><span class="sxs-lookup"><span data-stu-id="40972-161">Surface HUB device.</span></span>|
|<span data-ttu-id="40972-162">androidforwork</span><span class="sxs-lookup"><span data-stu-id="40972-162">androidForWork</span></span>|<span data-ttu-id="40972-163">17 </span><span class="sxs-lookup"><span data-stu-id="40972-163">17</span></span>|<span data-ttu-id="40972-164">Android for work デバイス。</span><span class="sxs-lookup"><span data-stu-id="40972-164">Android for work device.</span></span>|
|<span data-ttu-id="40972-165">androidenterprise</span><span class="sxs-lookup"><span data-stu-id="40972-165">androidEnterprise</span></span>|<span data-ttu-id="40972-166">18 </span><span class="sxs-lookup"><span data-stu-id="40972-166">18</span></span>|<span data-ttu-id="40972-167">Android エンタープライズデバイス。</span><span class="sxs-lookup"><span data-stu-id="40972-167">Android enterprise device.</span></span>|
|<span data-ttu-id="40972-168">blackberry</span><span class="sxs-lookup"><span data-stu-id="40972-168">blackberry</span></span>|<span data-ttu-id="40972-169">100</span><span class="sxs-lookup"><span data-stu-id="40972-169">100</span></span>|<span data-ttu-id="40972-170">Blackberry.</span><span class="sxs-lookup"><span data-stu-id="40972-170">Blackberry.</span></span>|
|<span data-ttu-id="40972-171">ヤシ</span><span class="sxs-lookup"><span data-stu-id="40972-171">palm</span></span>|<span data-ttu-id="40972-172">101</span><span class="sxs-lookup"><span data-stu-id="40972-172">101</span></span>|<span data-ttu-id="40972-173">ヤシ.</span><span class="sxs-lookup"><span data-stu-id="40972-173">Palm.</span></span>|
|<span data-ttu-id="40972-174">不明</span><span class="sxs-lookup"><span data-stu-id="40972-174">unknown</span></span>|<span data-ttu-id="40972-175">255</span><span class="sxs-lookup"><span data-stu-id="40972-175">255</span></span>|<span data-ttu-id="40972-176">デバイスの種類が不明であることを表します。</span><span class="sxs-lookup"><span data-stu-id="40972-176">Represents that the device type is unknown.</span></span>|





