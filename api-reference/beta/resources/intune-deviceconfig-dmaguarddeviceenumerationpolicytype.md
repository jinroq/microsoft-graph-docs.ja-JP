---
title: dmaGuardDeviceEnumerationPolicyType 列挙型
description: DmaGuardDeviceEnumerationPolicy の可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c46f7e49ad9d9ef31af4ee2d783f171b08c09f1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946883"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="af762-103">dmaGuardDeviceEnumerationPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="af762-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="af762-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af762-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af762-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af762-106">DmaGuardDeviceEnumerationPolicy の可能な値。</span><span class="sxs-lookup"><span data-stu-id="af762-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="af762-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="af762-107">Members</span></span>
|<span data-ttu-id="af762-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="af762-108">Member</span></span>|<span data-ttu-id="af762-109">値</span><span class="sxs-lookup"><span data-stu-id="af762-109">Value</span></span>|<span data-ttu-id="af762-110">説明</span><span class="sxs-lookup"><span data-stu-id="af762-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af762-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="af762-111">deviceDefault</span></span>|<span data-ttu-id="af762-112">.0</span><span class="sxs-lookup"><span data-stu-id="af762-112">0</span></span>|<span data-ttu-id="af762-113">既定値です。</span><span class="sxs-lookup"><span data-stu-id="af762-113">Default value.</span></span> <span data-ttu-id="af762-114">DMA が再マッピングされているデバイス互換性のないドライバーは、ユーザーが画面をロック解除した後にのみ列挙されます。</span><span class="sxs-lookup"><span data-stu-id="af762-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="af762-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="af762-115">blockAll</span></span>|<span data-ttu-id="af762-116">1-d</span><span class="sxs-lookup"><span data-stu-id="af762-116">1</span></span>|<span data-ttu-id="af762-117">DMA がマッピングされていないデバイス互換性のないドライバーは、いつでも DMA を開始して実行することはできません。</span><span class="sxs-lookup"><span data-stu-id="af762-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="af762-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="af762-118">allowAll</span></span>|<span data-ttu-id="af762-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="af762-119">2</span></span>|<span data-ttu-id="af762-120">すべての外部 DMA 対応 PCIe デバイスは、いつでも列挙されます。</span><span class="sxs-lookup"><span data-stu-id="af762-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




