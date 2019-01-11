---
title: androidDeviceOwnerBatteryPluggedMode 列挙型
description: Android デバイスの所有者の値、デバイスの電源に接続されているモードの状態です。
localization_priority: Normal
ms.openlocfilehash: 1ce7db347239a30b69fa8f22ff8b76804d7cdb52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843835"
---
# <a name="androiddeviceownerbatterypluggedmode-enum-type"></a><span data-ttu-id="d74be-103">androidDeviceOwnerBatteryPluggedMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="d74be-103">androidDeviceOwnerBatteryPluggedMode enum type</span></span>

> <span data-ttu-id="d74be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d74be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d74be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d74be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d74be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d74be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d74be-107">Android デバイスの所有者の値、デバイスの電源に接続されているモードの状態です。</span><span class="sxs-lookup"><span data-stu-id="d74be-107">Android Device Owner possible values for states of the device's plugged-in power modes.</span></span>
## <a name="members"></a><span data-ttu-id="d74be-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d74be-108">Members</span></span>
|<span data-ttu-id="d74be-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d74be-109">Member</span></span>|<span data-ttu-id="d74be-110">値</span><span class="sxs-lookup"><span data-stu-id="d74be-110">Value</span></span>|<span data-ttu-id="d74be-111">説明</span><span class="sxs-lookup"><span data-stu-id="d74be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d74be-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d74be-112">notConfigured</span></span>|<span data-ttu-id="d74be-113">0</span><span class="sxs-lookup"><span data-stu-id="d74be-113">0</span></span>|<span data-ttu-id="d74be-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="d74be-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="d74be-115">ac</span><span class="sxs-lookup"><span data-stu-id="d74be-115">ac</span></span>|<span data-ttu-id="d74be-116">1</span><span class="sxs-lookup"><span data-stu-id="d74be-116">1</span></span>|<span data-ttu-id="d74be-117">電源は、AC の充電器です。</span><span class="sxs-lookup"><span data-stu-id="d74be-117">Power source is an AC charger.</span></span>|
|<span data-ttu-id="d74be-118">usb</span><span class="sxs-lookup"><span data-stu-id="d74be-118">usb</span></span>|<span data-ttu-id="d74be-119">2</span><span class="sxs-lookup"><span data-stu-id="d74be-119">2</span></span>|<span data-ttu-id="d74be-120">電源は、USB ポートです。</span><span class="sxs-lookup"><span data-stu-id="d74be-120">Power source is a USB port.</span></span>|
|<span data-ttu-id="d74be-121">ワイヤレス</span><span class="sxs-lookup"><span data-stu-id="d74be-121">wireless</span></span>|<span data-ttu-id="d74be-122">3</span><span class="sxs-lookup"><span data-stu-id="d74be-122">3</span></span>|<span data-ttu-id="d74be-123">電源がワイヤレスです。</span><span class="sxs-lookup"><span data-stu-id="d74be-123">Power source is wireless.</span></span>|





