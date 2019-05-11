---
title: androidDeviceOwnerBatteryPluggedMode 列挙型
description: Android デバイスの所有者デバイスの電源モードの状態の値を指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d12dd2fcaa566892a5accb2c095ac19483fa69f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949186"
---
# <a name="androiddeviceownerbatterypluggedmode-enum-type"></a><span data-ttu-id="e23d3-103">androidDeviceOwnerBatteryPluggedMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="e23d3-103">androidDeviceOwnerBatteryPluggedMode enum type</span></span>

> <span data-ttu-id="e23d3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e23d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e23d3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e23d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e23d3-106">Android デバイスの所有者デバイスの電源モードの状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="e23d3-106">Android Device Owner possible values for states of the device's plugged-in power modes.</span></span>

## <a name="members"></a><span data-ttu-id="e23d3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e23d3-107">Members</span></span>
|<span data-ttu-id="e23d3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e23d3-108">Member</span></span>|<span data-ttu-id="e23d3-109">値</span><span class="sxs-lookup"><span data-stu-id="e23d3-109">Value</span></span>|<span data-ttu-id="e23d3-110">説明</span><span class="sxs-lookup"><span data-stu-id="e23d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e23d3-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e23d3-111">notConfigured</span></span>|<span data-ttu-id="e23d3-112">.0</span><span class="sxs-lookup"><span data-stu-id="e23d3-112">0</span></span>|<span data-ttu-id="e23d3-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="e23d3-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="e23d3-114">ac</span><span class="sxs-lookup"><span data-stu-id="e23d3-114">ac</span></span>|<span data-ttu-id="e23d3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e23d3-115">1</span></span>|<span data-ttu-id="e23d3-116">電力ソースは AC チャージャー。</span><span class="sxs-lookup"><span data-stu-id="e23d3-116">Power source is an AC charger.</span></span>|
|<span data-ttu-id="e23d3-117">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="e23d3-117">usb</span></span>|<span data-ttu-id="e23d3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e23d3-118">2</span></span>|<span data-ttu-id="e23d3-119">電源ソースは USB ポートです。</span><span class="sxs-lookup"><span data-stu-id="e23d3-119">Power source is a USB port.</span></span>|
|<span data-ttu-id="e23d3-120">通信</span><span class="sxs-lookup"><span data-stu-id="e23d3-120">wireless</span></span>|<span data-ttu-id="e23d3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e23d3-121">3</span></span>|<span data-ttu-id="e23d3-122">電力ソースはワイヤレス。</span><span class="sxs-lookup"><span data-stu-id="e23d3-122">Power source is wireless.</span></span>|




