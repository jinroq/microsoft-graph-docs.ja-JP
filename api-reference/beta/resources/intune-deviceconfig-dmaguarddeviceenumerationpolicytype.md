---
title: dmaGuardDeviceEnumerationPolicyType 列挙型
description: DmaGuardDeviceEnumerationPolicy の使用可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430454"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="1eed7-103">dmaGuardDeviceEnumerationPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1eed7-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="1eed7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1eed7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1eed7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eed7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1eed7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1eed7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eed7-107">DmaGuardDeviceEnumerationPolicy の使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="1eed7-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="1eed7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1eed7-108">Members</span></span>
|<span data-ttu-id="1eed7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1eed7-109">Member</span></span>|<span data-ttu-id="1eed7-110">値</span><span class="sxs-lookup"><span data-stu-id="1eed7-110">Value</span></span>|<span data-ttu-id="1eed7-111">説明</span><span class="sxs-lookup"><span data-stu-id="1eed7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eed7-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1eed7-112">deviceDefault</span></span>|<span data-ttu-id="1eed7-113">0</span><span class="sxs-lookup"><span data-stu-id="1eed7-113">0</span></span>|<span data-ttu-id="1eed7-114">既定値です。</span><span class="sxs-lookup"><span data-stu-id="1eed7-114">Default value.</span></span> <span data-ttu-id="1eed7-115">DMA の互換性のないドライバーを再割り当てを持つデバイスは、ユーザー画面のロックを解除した後にのみ列挙されます。</span><span class="sxs-lookup"><span data-stu-id="1eed7-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="1eed7-116">これ</span><span class="sxs-lookup"><span data-stu-id="1eed7-116">blockAll</span></span>|<span data-ttu-id="1eed7-117">1</span><span class="sxs-lookup"><span data-stu-id="1eed7-117">1</span></span>|<span data-ttu-id="1eed7-118">DMA の互換性のないドライバーを再割り当てを持つデバイスは、起動し、いつでも DMA を実行するのには許可されません。</span><span class="sxs-lookup"><span data-stu-id="1eed7-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="1eed7-119">すべて許可が次</span><span class="sxs-lookup"><span data-stu-id="1eed7-119">allowAll</span></span>|<span data-ttu-id="1eed7-120">2</span><span class="sxs-lookup"><span data-stu-id="1eed7-120">2</span></span>|<span data-ttu-id="1eed7-121">いつでもすべての外部 DMA 対応 PCIe デバイスが列挙されます。</span><span class="sxs-lookup"><span data-stu-id="1eed7-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




