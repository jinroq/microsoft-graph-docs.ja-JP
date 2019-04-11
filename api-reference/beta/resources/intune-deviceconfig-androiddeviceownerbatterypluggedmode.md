---
title: androidDeviceOwnerBatteryPluggedMode 列挙型
description: Android デバイスの所有者デバイスの電源モードの状態の値を指定できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ceaa8ee43139ab662c0d30a7b0b1d0d917dc1759
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782738"
---
# <a name="androiddeviceownerbatterypluggedmode-enum-type"></a><span data-ttu-id="4a5cf-103">androidDeviceOwnerBatteryPluggedMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="4a5cf-103">androidDeviceOwnerBatteryPluggedMode enum type</span></span>

> <span data-ttu-id="4a5cf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a5cf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a5cf-106">Android デバイスの所有者デバイスの電源モードの状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-106">Android Device Owner possible values for states of the device's plugged-in power modes.</span></span>

## <a name="members"></a><span data-ttu-id="4a5cf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a5cf-107">Members</span></span>
|<span data-ttu-id="4a5cf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a5cf-108">Member</span></span>|<span data-ttu-id="4a5cf-109">値</span><span class="sxs-lookup"><span data-stu-id="4a5cf-109">Value</span></span>|<span data-ttu-id="4a5cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="4a5cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a5cf-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4a5cf-111">notConfigured</span></span>|<span data-ttu-id="4a5cf-112">.0</span><span class="sxs-lookup"><span data-stu-id="4a5cf-112">0</span></span>|<span data-ttu-id="4a5cf-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="4a5cf-114">ac</span><span class="sxs-lookup"><span data-stu-id="4a5cf-114">ac</span></span>|<span data-ttu-id="4a5cf-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4a5cf-115">1</span></span>|<span data-ttu-id="4a5cf-116">電力ソースは AC チャージャー。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-116">Power source is an AC charger.</span></span>|
|<span data-ttu-id="4a5cf-117">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="4a5cf-117">usb</span></span>|<span data-ttu-id="4a5cf-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4a5cf-118">2</span></span>|<span data-ttu-id="4a5cf-119">電源ソースは USB ポートです。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-119">Power source is a USB port.</span></span>|
|<span data-ttu-id="4a5cf-120">通信</span><span class="sxs-lookup"><span data-stu-id="4a5cf-120">wireless</span></span>|<span data-ttu-id="4a5cf-121">1/3</span><span class="sxs-lookup"><span data-stu-id="4a5cf-121">3</span></span>|<span data-ttu-id="4a5cf-122">電力ソースはワイヤレス。</span><span class="sxs-lookup"><span data-stu-id="4a5cf-122">Power source is wireless.</span></span>|





