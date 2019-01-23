---
title: androidDeviceOwnerBatteryPluggedMode 列挙型
description: Android デバイスの所有者の値、デバイスの電源に接続されているモードの状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7291a687d5d179a1af2d7ba2dfdcd04b598b465f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392991"
---
# <a name="androiddeviceownerbatterypluggedmode-enum-type"></a><span data-ttu-id="c434f-103">androidDeviceOwnerBatteryPluggedMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="c434f-103">androidDeviceOwnerBatteryPluggedMode enum type</span></span>

> <span data-ttu-id="c434f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c434f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c434f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c434f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c434f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c434f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c434f-107">Android デバイスの所有者の値、デバイスの電源に接続されているモードの状態です。</span><span class="sxs-lookup"><span data-stu-id="c434f-107">Android Device Owner possible values for states of the device's plugged-in power modes.</span></span>

## <a name="members"></a><span data-ttu-id="c434f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c434f-108">Members</span></span>
|<span data-ttu-id="c434f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c434f-109">Member</span></span>|<span data-ttu-id="c434f-110">値</span><span class="sxs-lookup"><span data-stu-id="c434f-110">Value</span></span>|<span data-ttu-id="c434f-111">説明</span><span class="sxs-lookup"><span data-stu-id="c434f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c434f-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c434f-112">notConfigured</span></span>|<span data-ttu-id="c434f-113">0</span><span class="sxs-lookup"><span data-stu-id="c434f-113">0</span></span>|<span data-ttu-id="c434f-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="c434f-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="c434f-115">ac</span><span class="sxs-lookup"><span data-stu-id="c434f-115">ac</span></span>|<span data-ttu-id="c434f-116">1</span><span class="sxs-lookup"><span data-stu-id="c434f-116">1</span></span>|<span data-ttu-id="c434f-117">電源は、AC の充電器です。</span><span class="sxs-lookup"><span data-stu-id="c434f-117">Power source is an AC charger.</span></span>|
|<span data-ttu-id="c434f-118">usb</span><span class="sxs-lookup"><span data-stu-id="c434f-118">usb</span></span>|<span data-ttu-id="c434f-119">2</span><span class="sxs-lookup"><span data-stu-id="c434f-119">2</span></span>|<span data-ttu-id="c434f-120">電源は、USB ポートです。</span><span class="sxs-lookup"><span data-stu-id="c434f-120">Power source is a USB port.</span></span>|
|<span data-ttu-id="c434f-121">ワイヤレス</span><span class="sxs-lookup"><span data-stu-id="c434f-121">wireless</span></span>|<span data-ttu-id="c434f-122">3</span><span class="sxs-lookup"><span data-stu-id="c434f-122">3</span></span>|<span data-ttu-id="c434f-123">電源がワイヤレスです。</span><span class="sxs-lookup"><span data-stu-id="c434f-123">Power source is wireless.</span></span>|




