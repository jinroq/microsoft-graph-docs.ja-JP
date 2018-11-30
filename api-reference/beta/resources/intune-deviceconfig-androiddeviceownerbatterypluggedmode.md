---
title: androidDeviceOwnerBatteryPluggedMode 列挙型
description: Android デバイスの所有者の値、デバイスの電源に接続されているモードの状態です。
ms.openlocfilehash: 896e1c8a3a295a0d588a13b7a3e87eb1def02099
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067921"
---
# <a name="androiddeviceownerbatterypluggedmode-enum-type"></a><span data-ttu-id="75c42-103">androidDeviceOwnerBatteryPluggedMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="75c42-103">androidDeviceOwnerBatteryPluggedMode enum type</span></span>

> <span data-ttu-id="75c42-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75c42-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75c42-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75c42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75c42-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="75c42-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75c42-107">Android デバイスの所有者の値、デバイスの電源に接続されているモードの状態です。</span><span class="sxs-lookup"><span data-stu-id="75c42-107">Android Device Owner possible values for states of the device's plugged-in power modes.</span></span>
## <a name="members"></a><span data-ttu-id="75c42-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="75c42-108">Members</span></span>
|<span data-ttu-id="75c42-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="75c42-109">Member</span></span>|<span data-ttu-id="75c42-110">値</span><span class="sxs-lookup"><span data-stu-id="75c42-110">Value</span></span>|<span data-ttu-id="75c42-111">説明</span><span class="sxs-lookup"><span data-stu-id="75c42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c42-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="75c42-112">notConfigured</span></span>|<span data-ttu-id="75c42-113">0</span><span class="sxs-lookup"><span data-stu-id="75c42-113">0</span></span>|<span data-ttu-id="75c42-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="75c42-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="75c42-115">ac</span><span class="sxs-lookup"><span data-stu-id="75c42-115">ac</span></span>|<span data-ttu-id="75c42-116">1</span><span class="sxs-lookup"><span data-stu-id="75c42-116">1</span></span>|<span data-ttu-id="75c42-117">電源は、AC の充電器です。</span><span class="sxs-lookup"><span data-stu-id="75c42-117">Power source is an AC charger.</span></span>|
|<span data-ttu-id="75c42-118">usb</span><span class="sxs-lookup"><span data-stu-id="75c42-118">usb</span></span>|<span data-ttu-id="75c42-119">2</span><span class="sxs-lookup"><span data-stu-id="75c42-119">2</span></span>|<span data-ttu-id="75c42-120">電源は、USB ポートです。</span><span class="sxs-lookup"><span data-stu-id="75c42-120">Power source is a USB port.</span></span>|
|<span data-ttu-id="75c42-121">ワイヤレス</span><span class="sxs-lookup"><span data-stu-id="75c42-121">wireless</span></span>|<span data-ttu-id="75c42-122">3</span><span class="sxs-lookup"><span data-stu-id="75c42-122">3</span></span>|<span data-ttu-id="75c42-123">電源がワイヤレスです。</span><span class="sxs-lookup"><span data-stu-id="75c42-123">Power source is wireless.</span></span>|





