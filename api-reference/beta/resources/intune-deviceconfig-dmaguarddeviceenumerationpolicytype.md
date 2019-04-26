---
title: dmaGuardDeviceEnumerationPolicyType 列挙型
description: DmaGuardDeviceEnumerationPolicy の可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6910172ef4ab733b09d837dcc9a7196893402ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567159"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="58aff-103">dmaGuardDeviceEnumerationPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="58aff-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="58aff-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58aff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58aff-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58aff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58aff-106">DmaGuardDeviceEnumerationPolicy の可能な値。</span><span class="sxs-lookup"><span data-stu-id="58aff-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="58aff-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="58aff-107">Members</span></span>
|<span data-ttu-id="58aff-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="58aff-108">Member</span></span>|<span data-ttu-id="58aff-109">値</span><span class="sxs-lookup"><span data-stu-id="58aff-109">Value</span></span>|<span data-ttu-id="58aff-110">説明</span><span class="sxs-lookup"><span data-stu-id="58aff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58aff-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="58aff-111">deviceDefault</span></span>|<span data-ttu-id="58aff-112">.0</span><span class="sxs-lookup"><span data-stu-id="58aff-112">0</span></span>|<span data-ttu-id="58aff-113">既定値です。</span><span class="sxs-lookup"><span data-stu-id="58aff-113">Default value.</span></span> <span data-ttu-id="58aff-114">DMA が再マッピングされているデバイス互換性のないドライバーは、ユーザーが画面をロック解除した後にのみ列挙されます。</span><span class="sxs-lookup"><span data-stu-id="58aff-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="58aff-115">blockall</span><span class="sxs-lookup"><span data-stu-id="58aff-115">blockAll</span></span>|<span data-ttu-id="58aff-116">1 </span><span class="sxs-lookup"><span data-stu-id="58aff-116">1</span></span>|<span data-ttu-id="58aff-117">dma がマッピングされていないデバイス互換性のないドライバーは、いつでも dma を開始して実行することはできません。</span><span class="sxs-lookup"><span data-stu-id="58aff-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="58aff-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="58aff-118">allowAll</span></span>|<span data-ttu-id="58aff-119">2 </span><span class="sxs-lookup"><span data-stu-id="58aff-119">2</span></span>|<span data-ttu-id="58aff-120">すべての外部 DMA 対応 PCIe デバイスは、いつでも列挙されます。</span><span class="sxs-lookup"><span data-stu-id="58aff-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





